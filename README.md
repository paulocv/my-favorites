# My Favorite Picks

View the website: [paulocv.github.io/my-favorites/](https://paulocv.github.io/my-favorites/)

> [!NOTE]
> Modify the URL above to that of your website created with GitHub pages.

Example repository for a short course on Git and GitHub for scientists.

This site is built with Hugo and designed to be deployed with GitHub Pages using GitHub Actions.


# Notes for students

## Configuring your own webpage

In this repository on GitHub, click the "Use this template" green button on the top right of the page, then select "Create a new repository". You can name it as you wish, but it must have public visibility so the website can be published.

Once you have your own version, you can clone it locally and make changes using git. 

This project uses [hugo](https://gohugo.io/) to create a website. Before publishing it with GitHub pages (**required**), you must edit the `hugo.yaml` file. Replace the URL on `baseURL` with your own `https://[_username_].github.io/[_repo-name_]/`. This will also be the address of your website once published to GitHub Pages. You can optionally change the website name by editing the `title` field.


## Editing and previewing locally

You are encouraged to clone your own version of this repository to you local machine, so you can practice git locally and track your progress with commands like `git status`, `add`, `commit` and `push`.

It is possible to live-preview your changes as you make changes offline. To achieve this, you will have to setup and run a hugo server:

1. Install Hugo `0.134.0` or a compatible newer version. Tip: if you have conda, install it with `conda install conda-forge::hugo`. Otherwise check [https://gohugo.io/](https://gohugo.io/) for instructions.
2. From a terminal opened in the root directory of your local repo, run `hugo server --config hugo.yaml,hugo.local.yaml`.
3. Open the local address shown in the terminal. Most likely it will be [http://localhost:1313/](http://localhost:1313/). This will lead you to the offline preview of your website.


## Editing content

For simple content creation and editing, all you have to do is to modify files in the `content` directory of the repository.

- The `content/_index.md` file controls the homepage.
- Each markdown (`.md`) file in `content/picks` will automatically generate a favorite pick page. 
- You can control the title, summary sentence and tags of a favorite pick page by modifying the parameters between the "---" lines at the top of each file. 
  - This section is called "front matter" and is written in [yaml](https://yaml.org/) syntax.


## Example of a favorite pick file
```yaml
---
title: Example Pick
summary: One-sentence short description.
tags:
  - example
  - science
---

[Add the page content here.]
```

The home page table of contents updates automatically from the collection.

Only files inside `content/` become pages, so `README.md` stays as repository documentation and is not rendered as part of the website.




## Advanced editing

If you edit other files in the repository, you will be able to further customize the look and functioning of the webpage. Be curious and explore the possibilities! 👀 Use whatever help you need to make it look like your own.

Some examples:

- The `static/css/main.css` file controls the overall styling, from colors and fonts to responsive design in mobile devices. Play with the variables and see the effects.

- The `layouts` directory contains HTML templates that control _what_ goes _where_. If you dare changing these, you can further customize the structure of the website - or completely break it.

