# GH Pages No Jekyll
> A markdown-based docs on GitHub Pages which gets minimal styling from GitHub without a Jekyll theme

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/gh-pages-no-jekyll?include_prereleases=&sort=semver)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/releases/)
[![License - MIT](https://img.shields.io/badge/License-MIT-blue)](#license)


## Preview

<div align="center">
    <a href="https://michaelcurrin.github.io/gh-pages-no-jekyll/">
        <img src="/sample.png" alt="Sample screenshot" title="Sample screenshot" width="350" />
    </a>
</div>

<div align="center">

[![Use this template](https://img.shields.io/badge/Use_this_template-2ea44f?style=for-the-badge&logo=github)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/generate)

[![View site - GH Pages](https://img.shields.io/badge/View_site-GH_Pages-2ea44f?style=for-the-badge)](https://michaelcurrin.github.io/gh-pages-no-jekyll/)

</div>


## Features

- Template / quickstart
- Reference and tutorial
- Live demo


## About this repo

<!-- TODO move to docs -->

- A static site intended for docs or simple website. This project is great as reference or template for those.
- No custom styling such as CSS is used. Just plain markdown docs. GitHub automatically adds something like this to each page:
    - Site title
        - _gh-pages-no-jekyll_
    - CSS styling reference to make the page white and blue.
        - GitHub will create this file for you at the path `assets/css/style.css` and add a `link` stylesheet tag to a URL like this:
            - `/gh-pages-no-jekyll/assets/css/style.css?v=fb1...">`
        - Here is a [sample](https://michaelcurrin.github.io/gh-pages-no-jekyll/assets/css/style.css)
    - Footer
        - _This site is open source. Improve this page._
- No Jekyll theme or Liquid syntax is used. Where Liquid is actually used, it is code snippets and the `raw` tag is used to stop from rendering and giving an error on values no available).
- The Jekyll build is still run on Github Pages to convert markdown to HTML (a `.nojekyll` file would prevent this). 
- This project is **not** meant to be run locally (if there is a way, this is not covered here).

Read more on the live [demo site](https://michaelcurrin.github.io/gh-pages-no-jekyll/), which serves from the [docs](/docs/) directory.


## What about a Wiki?

<div align="center">

[![Project Wiki](https://img.shields.io/badge/Wiki-blue?style=for-the-badge)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/wiki)

</div>

As an alternative, consider using the Wiki feature on Github.

It will give a similar Github-styled experience of doc pages that separate from the code and files, but with the benefit of a menu. Note that a Wiki lives in its own repo, so updates made independently to the main part of the repo. A Wiki has a history, but does it not work Pull Requests and reviews so the edit process is different.


## License

Released under [MIT](/LICENSE) by [@MichaelCurrin](https://github.com/MichaelCurrin).
