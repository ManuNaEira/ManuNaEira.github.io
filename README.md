# ManuNaEira Personal blog / website <!-- omit in toc -->
This is the repository of my personal website / blog.
- [1. Requirements](#1-requirements)
  - [1.1. Environment](#11-environment)
  - [1.2. Site](#12-site)
  - [1.3. Post's format](#13-posts-format)
  - [1.4. Post's features](#14-posts-features)
- [2. Solutions](#2-solutions)
  - [2.1. GitHub pages & Jekyll build on server](#21-github-pages--jekyll-build-on-server)
    - [2.1.1. Requirements checklist](#211-requirements-checklist)
  - [2.2. GitHub pages & Jekyll build locally and pushed site](#22-github-pages--jekyll-build-locally-and-pushed-site)
## 1. Requirements
Following is the wish-list of features I would like to have available on the website. Every technology or solution adopted to build the website will be checked against them.
### 1.1. Environment
- [] **Test changes before deployment.**
### 1.2. Site
- [] **Good SEO performance.**
- [] **Search engine.**
- [] **Tags and collections.**
- [] **Light and dark mode.**
- [] **Multi-language.**
- [] **Get CV .pdf.**
### 1.3. Post's format
- [] **Code blocks - Format based on language.**
- [] **Code blocks - line numbers.**
- [] **Code blocks - Copy button.**
- [] **Math expressions.**
- [] **Callout sections.**
- [] **Toggle sections.**
- [] **Footnotes.**
  See [in this page](https://mmistakes.github.io/minimal-mistakes/markup-syntax-highlighting/#fnref:1) an example.
- [] **Web bookmarks, media embeds, etc. like Notion.**
### 1.4. Post's features
- [] **Table of Contents always visible while scrolling down.**
- [] **Button return to top in long posts.**
- [] **Both published and last modified date.**

## 2. Solutions
### 2.1. GitHub pages & Jekyll build on server
Using the [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) theme.
#### 2.1.1. Requirements checklist
##### 2.1.1.1. Environment
- [x] **Test changes before deployment.** By using branches and building Jekyll locally.
##### 2.1.1.2. Site
- [] **Good SEO performance.**
- [x] **Search engine.**
- [x] **Tags and collections.**
- [] **Light and dark mode.**
- [] **Multi-language.**
- [] **Get CV .pdf.**
  Looks it could be possible [link](https://jekyllrb.com/docs/posts/#including-images-and-resources). But note it won't be efficient to store the
  .pdf file directly in Git and keep updating it.
##### 2.1.1.3. Post's format
- [x] **Code blocks - Format based on language.**
- [x] **Code blocks - line numbers.**
- [] **Code blocks - Copy button.**
- [x] **Math expressions.** Not by default. But there is a workaround to achieve it: Adding Mathjax script to `_includes` folder. [[link 1](http://disq.us/p/27j4kl9)], [[link 2, from the minimal-mistakes theme author](https://github.com/mmistakes/minimal-mistakes/issues/735#issuecomment-269500816)].
- [x] **Callout sections.**
- [?] **Toggle sections.**
  Partial support. Toggle button is seen but the content inside is not parsed by markdown. We could use the Liquid filter `markdownify` to capture the inside of the toggle section and force it to be parsed as markdown (see [here](https://mmistakes.github.io/minimal-mistakes/post%20formats/post-notice/) an example for callouts/notify sections), but it is not working so far, at least for headings `#`.
  Another option is to use HTML buttons like shown [here](http://tomnorian.com/toggle-code-display-jekyll.html).
- [x] **Footnotes.**
  See [in this page](https://mmistakes.github.io/minimal-mistakes/markup-syntax-highlighting/#fnref:1) an example.
- [] **Web bookmarks, media embeds, etc. like Notion.**
##### 2.1.1.4. Post's features
- [x] **Table of Contents always visible while scrolling down.**
- [] **Button return to top in long posts.**
- [?] **Both published and last modified date.**
  Last modified date available, but it appears at the end of the post and not at
  the very beginning as the main date related to the post, as it can be seen [in
  this one](docs/_posts/2019-04-18-welcome-to-jekyll.md).
### 2.2. GitHub pages & Jekyll build locally and pushed site

