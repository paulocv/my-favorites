# Favorite Aircraft Picks

Example repository for a short course on Git and GitHub for scientists.

This site is built with Jekyll and designed to be deployed with GitHub Pages using GitHub Actions.


## Notes for students

Add new favorite picks by creating Markdown files in [`_picks/`](/Users/pventura/NonCloudStorage/Work_related/GitHub_for_scientists/my-favorites/_picks), with the following template:

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


## Local preview

1. Install Ruby and Bundler.
2. Run `bundle install`.
3. Run `bundle exec jekyll serve`.
4. Open the local address shown in the terminal.

## What this example shows

- A simple Jekyll site with a custom collection
- Individual pages for favorite picks
- A shared layout for pick pages
- An automatically generated table of contents on the home page
- A GitHub Actions workflow for Pages deployment

