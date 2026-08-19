# SuDIS@ZJU website

This repository contains the public website for the Sustainable Data Intelligence and Data Systems (SuDIS) research group at Zhejiang University.

The site is built with [Hugo](https://gohugo.io/) and the [Hugo Blox Builder](https://hugoblox.com/), then deployed to GitHub Pages from `main`.

## Local preview

Install Hugo Extended and run:

```bash
hugo server --environment development --baseURL http://localhost:1313/ --gc --disableFastRender
```

The production build is:

```bash
hugo --gc --minify
```

## Public content

The public site includes bilingual group information, member profiles, research publications, and selected news. Publication pages and `publications.bib` are generated from the project's maintained publication records; generated pages should not be edited manually.

## License

Site content is published under the Creative Commons Attribution-ShareAlike 4.0 International License unless otherwise noted. The site's source configuration and templates remain under the repository's MIT license.
