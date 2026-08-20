---
name: sudis-site-maintainer
description: Safely maintain the SuDIS-ZJU public Hugo website through source-aware edits, validation, and pull requests. Use this skill whenever a user asks to update the SuDIS website, add or revise News, correct a student profile or publication record, change navigation or templates, run site checks, or prepare a PR. It distinguishes public-only edits from private-synchronizer work and prevents hand-editing generated author and publication pages as if they were source data.
compatibility: Requires Git and Hugo Extended 0.144.2 for public-site checks. GitHub CLI (`gh`) is optional for PR operations. The private synchronizer is available only to authorized maintainers.
---

# SuDIS Site Maintainer

Use this skill to make small, reviewable, source-aware changes to the SuDIS-ZJU website. The site is a Hugo project with bilingual homepage and News content, English-only People and Publication navigation, and generated author/publication records.

The central rule is: **edit the correct source, validate the rendered result, and deliver the change through a PR**.

## 1. Operating mode

First determine which of these modes is available:

| Mode | Available inputs | Allowed work |
|---|---|---|
| Public-only | `SuDIS-ZJU.github.io` | News, public prose, templates, styles, links, accessibility, and documented public assets |
| Private-sync | Public repo plus authorized `SuDIS-ZJU-site-private` | Vault projection, student allowlist, paper metadata, translations, generated pages, full release checks |
| Review-only | No write authorization | Inspect, explain, and prepare a patch or checklist; do not commit or push |

Never infer private-sync authorization from the presence of a local directory. Confirm that the user is an authorized maintainer before reading or changing private Vault-derived data.

## 2. Start every task with a safety check

1. Locate the public repository root with `git rev-parse --show-toplevel`.
2. Read the repository `AGENTS.md`, `README.md`, and `CONTRIBUTING.md` when present.
3. Check the current branch and worktree:

   ```bash
   git branch --show-current
   git status --short
   git log --oneline -5
   ```

4. Preserve unrelated user changes. Do not reset, clean, discard, or overwrite them.
5. If the current branch is `main`, create a task branch before editing:

   ```bash
   git switch -c <type>/<short-description>
   ```

6. Classify the requested change before touching files. If it concerns an author or publication record and private-sync mode is unavailable, stop editing the generated page and prepare an Issue or maintainer request with the evidence needed for a source update.

## 3. Change routing

Use this routing table to choose the source of truth:

| Request | Preferred source | Public-only action |
|---|---|---|
| Add or revise a News report | `content/en/post/` and `content/zh/post/` | Edit both language files when bilingual News is requested |
| Fix layout, navigation, footer, alt text, or CSS | `layouts/`, `assets/`, `config/` | Edit the template or configuration, not `public/` |
| Correct a student name, cohort, role, employment, or contact | Private student source / `config/site-sync.json` | Open an Issue or ask an authorized maintainer to update the private source |
| Correct DOI, author list, venue, year, ranking, or citation key | Vault paper record / private translation table | Provide authoritative evidence; do not hand-edit generated paper pages |
| Add a preprint | Private preprint registry, then synchronizer | Ask a maintainer unless the public source is explicitly designated for direct editing |
| Remove a public page | Private allowlist or maintainer-approved source change | Never delete a generated page directly |

Generated files include `content/*/authors/*/_index.md`, structured `content/*/publication/*` records, and `publications.bib`. A direct edit to these files may appear to work but will be overwritten by the next synchronization.

## 4. Content safety rules

- Do not publish Vault paths, internal notes, unpublished work, private evaluations, credentials, or personal contact details without explicit authorization.
- Do not invent Chinese titles, abstracts, awards, acceptance status, rankings, experimental numbers, employment, or supervision relationships.
- Keep preprints explicitly labeled as preprints or open-source results.
- Preserve stable paper IDs, aliases, citation keys, DOI values, author order, and external URLs unless the maintainer explicitly approves a compatibility change.
- Keep paper author display in English. Link to a Chinese student profile only when the existing site policy provides that profile.
- Keep bilingual News semantically aligned and professionally written. Do not use unreviewed machine translation for academic claims.
- Use relative or site-root-relative internal links, never hard-coded production domains or temporary localhost links in content.
- Give every new image meaningful alt text, verify its license/source, and avoid committing oversized originals.
- Never commit `.env`, keys, tokens, `public/`, build caches, browser logs, screenshots, or private backups.

## 5. Public-only implementation workflow

For News, public copy, templates, styles, links, and accessibility fixes:

1. Create a focused branch from the latest `main`.
2. Make the smallest source edit with `apply_patch` or the repository's normal editor.
3. Keep English and Chinese News files aligned when the task is bilingual. People and Publication are not automatically bilingual.
4. Build into a temporary destination so stale files do not hide route problems:

   ```bash
   build_dir="$(mktemp -d /tmp/sudis-site-check.XXXXXX)"
   hugo --gc --minify --destination "$build_dir"
   git diff --check
   ```

5. Inspect the rendered pages relevant to the change. At minimum check the homepage, News index, the changed page, and any language or link route affected.
6. Review the diff for private paths, generated-file edits, absolute internal links, accidental deletions, and unrelated formatting changes.

Do not use `rm -rf`, `git clean`, `git reset --hard`, or `git checkout --` to make a build pass. Preserve the worktree and ask the user before any material deletion.

## 6. Authorized private-sync workflow

Only an authorized maintainer may use this workflow. Run it from `SuDIS-ZJU-site-private`:

```bash
./bin/sitectl plan
./bin/sitectl stage
./bin/sitectl verify
./bin/sitectl verify --priority-translations
./bin/sitectl test
./bin/sitectl release-check
hugo --gc --minify
```

Before `apply --confirm-removals`:

1. Read `plan` output and confirm public IDs, removed IDs, paper counts, preprints, and News records.
2. Confirm every removal is intentional and in scope.
3. Confirm a recoverable backup is created.
4. Review the generated diff for private fields, internal paths, and management metadata.
5. Run the complete test suite again after applying.

The removal-capable command is:

```bash
./bin/sitectl apply --confirm-removals
```

Never run it merely to make a local page disappear. A source-level removal decision and a backup are required.

## 7. PR workflow

Commit only the files belonging to the task:

```bash
git add <explicit-files>
git diff --cached --check
git commit -m "<type>(<scope>): <imperative summary>"
git push -u origin <branch-name>
```

Use one topic per PR. Recommended commit prefixes are `docs`, `fix`, `feat`, `chore`, and `refactor`.

The PR description should include:

- Summary and affected routes;
- Source of every factual change;
- Whether English and Chinese content are both affected;
- Whether stable URLs, aliases, DOI, or citation keys change;
- Commands run and their results;
- Screenshots for visual or responsive changes;
- Any item requiring PI confirmation.

Only create or push a PR when the user explicitly requests delivery. Otherwise leave the validated branch and report the exact files and commands.

## 8. Review checklist

Before declaring the work ready:

- [ ] Branch is not `main`.
- [ ] No unrelated worktree changes were overwritten.
- [ ] Correct source was edited rather than a generated output.
- [ ] Public/private boundary is preserved.
- [ ] No unsupported factual claim was added.
- [ ] Internal links do not point to production or temporary localhost URLs.
- [ ] Hugo build succeeds in a fresh destination.
- [ ] `git diff --check` succeeds.
- [ ] The PR has a focused title, evidence, test commands, and risk notes.
- [ ] `build-and-audit` passes before merge.

## 9. Response format

When reporting back to the student or maintainer, use this compact structure:

1. **Result**: what changed or why the change was blocked.
2. **Source**: files or private source records edited.
3. **Validation**: exact commands and pass/fail result.
4. **PR**: branch, commit, and PR URL if delivery was requested.
5. **Follow-up**: unresolved facts, required PI confirmation, or next action.

When a request conflicts with the source-of-truth or privacy rules, explain the conflict and prepare a safe Issue/PR description instead of silently modifying generated output.
