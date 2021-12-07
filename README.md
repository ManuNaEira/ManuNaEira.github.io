# ManuNaEira Personal blog / website
This is the repository of my personal website / blog.
## Requirements
Following is the wishlist of features I would like to have available on the website. Every technology or solution adopted to build the website will be confronted against them.
- [] **Possibility to test changes before deployment.**
- [] **Powerful search engine.**
- [] **Tags and collections.**
- [] **Light and dark mode.**
- [] **Multi-language.**
- [] **Table of Contents always visible while scrolling down.**
- [] **Code blocks - Format based on language.**
- [] **Code blocks - lines.**
- [] **Code blocks - Copy button.**
- [] **Math expressions.**
- [] **Callout sections.**
- [] **Toggle sections.**
- [] **Footnotes.**
  See [in this page](https://mmistakes.github.io/minimal-mistakes/markup-syntax-highlighting/#fnref:1) an example
- [] **Get CV .pdf.**
- [] **Button return to top in long posts.**
- [] **Web bookmarks like Notion.**
- [] **Good SEO performance.**
## Solutions
### GitHub pages & Jekyll build on server
Tried using the [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) theme.
- [x] **Possibility to test changes before deployment.**
  By using branches and building Jekyll locally.
- [x] **Powerful search engine**
- [x] **Tags and collections**
- [] **Light and dark mode**
- [] **Multi-language**
- [x] **Table of Contents always visible while scrolling down**
- [x] **Code blocks - Format based on language**
- [x] **Code blocks - lines**
- [] **Code blocks - Copy button**
- [x] **Math expressions**
   Not by default. But there is a workaround to achieve it: Adding Mathjax script to `_includes` folder. [[link 1](http://disq.us/p/27j4kl9)], [[link 2, from the minimal-mistakes theme author](https://github.com/mmistakes/minimal-mistakes/issues/735#issuecomment-269500816)].
- [] **Toggle sections**
  Partial support. Toggle button is seen but the content inside is not parsed by markdown. We could use the Liquid filter `markdownify` to capture the inside of the toggle section and force it to be parsed as markdown (see [here](https://mmistakes.github.io/minimal-mistakes/post%20formats/post-notice/) an example for callouts/notify sections), but it is not working so far, at least for headings `#`.
  Another option is to use HTML buttons like shown [here](http://tomnorian.com/toggle-code-display-jekyll.html).
- [] **Get CV .pdf**
  Looks it could be possible [link](https://jekyllrb.com/docs/posts/#including-images-and-resources).
- [] **Button return to top in long posts**
- [] **Web bookmarks like Notion**
- [] **Good SEO performance**
### GitHub pages & Jekyll build locally and pushed site

