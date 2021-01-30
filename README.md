# GH Pages No Jekyll
> Template for a markdown-based docs site hosted on GH Pages

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/gh-pages-no-jekyll?include_prereleases=&sort=semver)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)


## Preview

<div align="center">
    <a href="https://michaelcurrin.github.io/gh-pages-no-jekyll/">
        <img src="/sample.png" alt="Sample screenshot" title="Sample screenshot" width="350" />
    </a>
</div>

<br>

<div align="center">

[![View site - GH Pages](https://img.shields.io/badge/View_site-GH_Pages-blue?style=for-the-badge)](https://michaelcurrin.github.io/gh-pages-no-jekyll/)

[![Use this template](https://img.shields.io/badge/Use_this_template-Generate-2ea44f?style=for-the-badge&logo=github)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/generate)

</div>


## Features

- The docs site use a default minimal theme provided by GitHub. 
- Great for a light docs site that doesn't need coding experience to setup or work on.
- Works without Jekyll templating, a Jekyll theme or Jekyll config.


## How to use this project

- Template for a new project
- Reference and tutorial content
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
