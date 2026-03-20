# Favorite Aircraft Picks

View the website: [paulocv.github.io/my-favorites/](https://paulocv.github.io/my-favorites/)

Example repository for a short course on Git and GitHub for scientists.

This site is built with Hugo and designed to be deployed with GitHub Pages using GitHub Actions.


## Notes for students

Add new favorite picks by creating Markdown files in [`content/picks/`](/Users/pventura/NonCloudStorage/Work_related/GitHub_for_scientists/my-favorites/content/picks), with the following template:

```yaml
---
title: Example Pick
summary: One-sentence description of why this is a favorite.
tags:
  - example
  - science
---

[Add the page content here.]
```

The home page table of contents updates automatically from the collection.

Only files inside `content/` become pages, so `README.md` stays as repository documentation and is not rendered as part of the website.


## Local preview

1. Install Hugo `0.134.0` or a compatible newer version.
2. Run `hugo server --config hugo.yaml,hugo.local.yaml` for local development at `http://localhost:1313/`.
3. Open the local address shown in the terminal.

## What this example shows

- A simple Hugo site with a section for favorite picks
- Individual pages for favorite picks
- A shared layout for pick pages
- An automatically generated table of contents on the home page
- A GitHub Actions workflow for Pages deployment
