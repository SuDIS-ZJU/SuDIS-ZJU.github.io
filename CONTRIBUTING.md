# SuDIS 网站维护与权限规范

本文档适用于 SuDIS-ZJU 网站源码仓库及其相关的私有内容同步流程。目标是让成员能够安全、可追溯地维护网站，同时避免未经确认的公开、生成内容漂移和主分支破坏。

## 1. 基本原则

1. **最小权限**：只授予完成工作所需的最低 GitHub 权限。
2. **PR 优先**：任何内容或代码变更都通过 Pull Request（PR）进入 `main`，禁止直接推送 `main`。
3. **源数据优先**：作者、论文和公开名单由私有同步器生成。生成页面不是事实源，禁止只修改生成结果来“修复”内容。
4. **公开前审查**：公开信息必须已经得到成员本人或课题组负责人的确认；未公开研究、内部链接和私有路径不得进入公开仓库。
5. **可回滚**：一个 PR 只处理一个主题，提交保持小而清晰，必要时能够单独回滚。
6. **事实优先于完整**：不确定的信息留空或提交待确认请求，不猜测、不补写、不把预印本写成已录用论文。

## 2. 仓库和数据边界

SuDIS 网站维护分为两个边界：

| 区域 | 主要内容 | 谁可以修改 |
|---|---|---|
| 公开仓库 `SuDIS-ZJU.github.io` | Hugo 模板、公开页面、公开 News、静态资源 | 维护者和获授权的贡献者，通过 PR 修改 |
| 私有同步仓库 `SuDIS-ZJU-site-private` | Vault 投影、公开名单、论文源数据、翻译表、生成器和审计脚本 | PI 指定的维护者；学生只有在单独获授权后才能访问 |
| 私有 Vault | 学生原始资料、内部项目、未公开论文和管理信息 | 仅按 Vault 自身权限访问，不能复制到公开仓库 |

公开仓库不应出现以下内容：

- `/Users/...`、`/Zspace/...` 等本机或 Vault 路径；
- 私有同步仓库的配置、日志、备份和管理字段；
- 未公开项目、内部会议记录、未授权联系方式；
- API Token、密码、私钥、Cookie、云服务凭据；
- 仅供内部使用的图片、原始数据和文档。

## 3. GitHub 权限分级

### 3.1 PI / Repository Owner

PI 或仓库 Owner 负责：

- 管理仓库成员、Teams、分支保护和 GitHub Actions 权限；
- 决定哪些学生、论文、项目和联系方式可以公开；
- 审批涉及个人简介、论文归属、对外声明和删除操作的 PR；
- 合并高风险 PR、处理安全事件和恢复错误发布；
- 管理私有同步仓库和 Vault 的访问权限。

### 3.2 Maintainer（网站维护者）

建议授予 GitHub **Write** 权限，不授予维护者直接绕过分支保护的权限。维护者可以：

- 创建分支、推送分支和提交 PR；
- 运行 Hugo 构建和公开仓库审计；
- 审核普通排版、News、链接和资源优化 PR；
- 在 PI 授权下运行私有同步器并更新生成内容；
- 在至少一名合适审阅者批准后合并普通 PR。

维护者不得：

- 直接推送 `main`；
- 未经确认执行包含移除操作的同步；
- 私自扩大公开学生、论文、项目或联系方式范围；
- 通过修改 CI、分支保护或权限设置绕过审核。

### 3.3 Student Contributor（学生贡献者）

学生默认使用 **Read** 权限或 Fork 工作流。若需要在本仓库创建分支并提交 PR，可授予 **Write** 权限，但仍必须遵守：

- 不能直接写入 `main`；
- 不能修改分支保护、Actions 权限或仓库 Secrets；
- 不能自行合并包含本人信息或本人论文的 PR；
- 不能把私有 Vault 内容复制到公开仓库；
- 不能提交未经确认的个人邮箱、电话、简历或就业信息。

学生若没有私有同步仓库权限，可以通过公开仓库 PR 维护 News、已确认的公开文案、排版和链接；论文与作者源数据应提交 Issue 或请求 PI/维护者更新私有源，再由同步器生成。

### 3.4 External Contributor

外部贡献者使用 Fork + PR，不授予仓库写权限。外部贡献者可以修复公开链接、拼写、无障碍属性和明显的排版问题，但不能新增成员、修改公开名单或发布未核实成果。

### 3.5 GitHub Actions Bot

Actions 只负责构建和审计，不应拥有写入 `main` 的权限。任何自动部署必须以合并后的 `main` 为输入，并保留构建日志。

### 3.6 PI 应配置的仓库保护

在 GitHub 的 **Settings → Collaborators and teams** 中：

- 学生贡献者：`Read`（Fork 工作流）或 `Write`（需要在本仓库创建分支时）；
- 网站维护者：`Write`；
- PI/Owner：`Admin`；
- 不给学生 `Maintain` 或 `Admin`，除非有明确的长期运维授权。

在 **Settings → Branches → Branch protection rules** 为 `main` 配置：

- Require a pull request before merging；
- Require at least one approval；
- Require conversation resolution before merging；
- Require status checks to pass，选择 `build-and-audit`；
- Require branches to be up to date before merging；
- Restrict who can push to matching branches，原则上不允许学生直接推送；
- 禁止 force push 和 branch deletion；
- 不允许 PR 作者自审自合；
- 对 workflow、权限和分支保护变更要求 PI 审核。

如果仓库启用了 GitHub Environments 或 Pages 部署保护，应只允许 `main` 触发正式部署，并限制 Secrets 的读取范围。

## 4. 分支和命名规范

本地开始工作前，先同步 `main`：

```bash
git switch main
git pull --ff-only origin main
git switch -c <type>/<short-description>
```

分支命名建议：

| 类型 | 示例 |
|---|---|
| News | `news/forcing-kv-report` |
| 个人资料 | `profile/yongqin-xu-correction` |
| 论文元数据 | `paper/c070-venue-correction` |
| 页面功能 | `fix/english-only-navigation` |
| 资源优化 | `chore/compress-avatars` |

分支应从最新 `main` 创建，不要在已经合并的旧分支上继续堆叠新工作。需要更新 PR 时，继续推送同一分支即可，不要反复创建重复 PR。

## 5. 哪些内容可以提交 PR

### 5.1 学生可以直接维护的内容

- News 的英文和中文稿件；
- 已经公开且事实明确的会议、奖项、项目和论文报道；
- 页面拼写、链接、标题层级、无障碍属性和响应式样式；
- 已经确认的公开图片及其版权说明、替代文本；
- 不涉及事实变更的 CSS、Hugo 模板和审计测试。

### 5.2 必须先经过 PI/维护者确认的内容

- 新增或移除学生、校友、PI 或其他成员；
- 修改姓名、年级、学位类型、指导关系、就业去向或联系方式；
- 修改论文作者、年份、DOI、venue、CCF/CORE/影响因子等元数据；
- 新增项目、资助来源、合作企业和量化成果；
- 发布中文论文标题、关键词或摘要；
- 删除稳定 URL、alias、BibTeX citation key 或公开页面；
- 任何可能造成宣传 overclaim 的表述。

### 5.3 禁止直接修改的生成内容

以下文件通常由私有同步器生成，学生不应只在公开仓库中手工修改：

- `content/*/authors/*/_index.md` 中的结构化个人资料；
- `content/*/publication/*/index.md` 和对应 `cite.bib`；
- `publications.bib`；
- 同步器覆盖的首页项目表、学生论文列表和论文作者链接。

如果发现这些页面有误，请在 PR 或 Issue 中提供：页面 URL、正确内容、证据来源、是否需要中英文同步，以及是否涉及稳定 URL。维护者确认后应修改私有源并重新生成。

## 6. 内容和学术事实规范

### 6.1 论文

- 作者顺序、论文 ID、年份、DOI、BibTeX key 和稳定 URL 必须保持兼容；
- DOI 只保留一个公开入口；
- 预印本明确标注为 `Preprint` 或 `Open-source result`，不能写成已录用论文；
- 会议、期刊、Demo、Workshop、Tutorial 等类型必须与论文源数据一致；
- CCF、CORE、影响因子等等级信息必须有可核验来源；
- 不要为了“中文化”而编造标题、摘要或实验结论；
- 论文详情页中的作者显示遵循英文作者名规范，学生个人页面可通过链接进入中文界面。

### 6.2 News

- 只报道已经公开的成果和事件；
- 中文 News 不是逐字机器翻译，术语、会议名称和结论应人工审核；
- 不新增原文没有的实验数字、奖项级别、录用状态或产业影响；
- 文章应包含必要背景，但保持客观、克制、可追溯；
- 来源链接应指向公开论文、项目仓库、学校/会议页面或已授权媒体报道。

### 6.3 个人资料

- 个人姓名、头像、邮箱、GitHub、Google Scholar 等信息须经本人确认或已有公开授权；
- 学生页面的研究兴趣应保持语言一致，中文页使用完整中文，英文页使用完整英文；
- 就业、实习、年级、毕业身份和 co-supervised 标记必须有 PI 或本人确认；
- 不公开私人手机号、家庭地址、身份证件、内部评价和未公开 offer。

### 6.4 链接和资源

- 站内链接优先使用相对或站点根相对路径，不能写死线上域名；
- 内容中不得残留 `localhost`、临时预览地址或本机文件路径；
- 外部链接使用 HTTPS，提交前确认目标页面可访问；
- 图片应有明确来源和 `alt` 文本；不提交超过项目门限的大型原图；
- 不提交 `public/`、构建缓存、Playwright 日志和临时截图。

## 7. 学生提交 PR 的标准流程

### 7.1 Fork 工作流（推荐）

```bash
git clone https://github.com/<your-account>/SuDIS-ZJU.github.io.git
cd SuDIS-ZJU.github.io
git remote add upstream https://github.com/SuDIS-ZJU/SuDIS-ZJU.github.io.git
git fetch upstream
git switch -c news/my-update upstream/main
```

完成修改后：

```bash
hugo --gc --minify --destination /tmp/sudis-site-build
git diff --check
git status --short
git add <明确的文件>
git commit -m "docs(news): add <short description>"
git push -u origin news/my-update
```

然后在 GitHub 上创建 PR，目标仓库为 `SuDIS-ZJU/SuDIS-ZJU.github.io`，目标分支为 `main`。

### 7.2 同仓库分支工作流

只有获得 Write 权限的成员使用此方式：

```bash
git clone https://github.com/SuDIS-ZJU/SuDIS-ZJU.github.io.git
cd SuDIS-ZJU.github.io
git switch main
git pull --ff-only origin main
git switch -c profile/my-correction
```

PR 创建后，后续修改继续推送到同一分支：

```bash
git add <明确的文件>
git commit -m "fix(profile): correct student metadata"
git push
```

## 8. 私有同步器工作流

只有 PI 指定的私有仓库维护者执行以下流程。学生若没有私有仓库权限，不要自行复制 Vault 数据。

```bash
cd SuDIS-ZJU-site-private
./bin/sitectl plan
./bin/sitectl stage
./bin/sitectl verify
./bin/sitectl verify --priority-translations
./bin/sitectl test
./bin/sitectl release-check
hugo --gc --minify
```

只有在明确确认名单、页面删除和公开字段变更后，才执行：

```bash
./bin/sitectl apply --confirm-removals
```

执行 `apply` 前必须：

1. 阅读 `plan` 输出，确认 `public_ids`、`remove_ids`、论文数量和预印本数量；
2. 确认所有移除项都属于本次任务；
3. 确认同步器已经创建可恢复备份；
4. 检查生成 diff，不包含私有来源、内部路径或管理字段；
5. 运行完整测试后再把公开仓库改动推送到 PR。

## 9. PR 描述和检查清单

每个 PR 应说明：

- 修改目的和影响页面；
- 是否涉及作者、论文、News、导航、模板或图片；
- 事实来源和人工确认人；
- 是否改变稳定 URL、alias、DOI 或 citation key；
- 本地验证命令和结果；
- 是否需要中英文同步；
- 是否存在待确认信息或后续工作。

提交前检查：

- [ ] 分支来自最新 `main`；
- [ ] PR 只包含一个逻辑主题；
- [ ] 没有私有路径、凭据、Vault 字段或临时文件；
- [ ] 没有直接修改不应手工维护的生成页面；
- [ ] 站内链接、外部链接和图片均已检查；
- [ ] `hugo --gc --minify` 通过；
- [ ] `git diff --check` 通过；
- [ ] `build-and-audit` 通过；
- [ ] PR 描述已填写来源、验证和风险；
- [ ] 涉及个人事实时已获得本人或 PI 确认。

## 10. 审核和合并规则

### 普通低风险 PR

适用于拼写、排版、链接、alt 文本和不改变事实的样式修改：

- 至少一名维护者审核；
- CI 通过；
- 无敏感信息；
- 可使用 Squash and merge。

### 内容和事实 PR

适用于 News、个人资料、论文元数据、项目和奖项：

- 至少一名维护者审核；
- 涉及本人信息时由本人确认，涉及课题组事实时由 PI 或指定维护者确认；
- 论文元数据应核对 DOI、出版方、DBLP、arXiv 或项目仓库；
- CI 通过后再合并。

### 高风险 PR

适用于删除页面、修改稳定 URL、修改 CI、权限、工作流、分支保护或公开范围：

- 必须由 PI 审核；
- 至少保留一名额外维护者复核；
- 需要在 PR 中写明回滚方案；
- 不允许学生单独合并。

## 11. 错误发布和回滚

发现错误后，先判断是否需要立即处理：

1. **隐私或安全问题**：立即通知 PI，暂停进一步传播，必要时撤回或修订页面，并检查 Git 历史影响。
2. **事实错误但不涉及安全**：创建修正 PR，引用原页面和权威来源，优先通过正常审核合并。
3. **构建失败**：查看 `build-and-audit` 日志，修复当前 PR，不要绕过检查直接推送 `main`。
4. **错误合并**：优先提交反向修复 PR；只有在明确授权下才进行历史重写。

不要使用 `git push --force`、`git reset --hard` 或删除远端分支来掩盖问题。

## 12. 权限申请和离组处理

权限申请应由 PI 或维护者记录以下信息：

- GitHub 用户名和学校/课题组身份；
- 需要访问的仓库和所需任务；
- 是否需要私有同步仓库或 Vault 访问；
- 权限起止时间和审批人。

学生毕业、离组或任务结束后，应及时：

- 移除不再需要的仓库和 Vault 权限；
- 撤销临时 Token、Deploy Key 和本地凭据；
- 关闭未完成的临时分支或转交维护者；
- 对仍需维护的 PR 补充交接说明。

## 13. 最简学生速查版

1. 不直接改 `main`，先从最新 `main` 建分支。
2. News、排版、链接和无障碍问题可以直接提 PR。
3. 学生和论文事实先确认，再改；生成页面不要手工长期维护。
4. 不提交私有路径、Vault 内容、临时文件和凭据。
5. 本地运行 Hugo 和 `git diff --check`。
6. 一个 PR 只做一件事，写清来源和验证结果。
7. 等 CI 和维护者审核通过后，由 PI/维护者合并到 `main`。

如有疑问，优先提交 Issue 或在 PR 中标注 `需要 PI 确认`，不要自行猜测或扩大公开范围。
