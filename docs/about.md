# **About**

This project is a built around GitHub's functionality which lets you use GitHub Pages to render markdown (or HTML) files as a static website, from your root or `docs` folder.

Jekyll is still actually used to convert the files, but the project works with **no** typical Jekyll files such as layouts, themes, gems or configs. Github handles the CSS styling with a basic blue and white theme.

This means it is very **light**, as you only write content.

Note you can still use Jekyll Liquid templating. But the idea for this project is to avoid it and make a plain markdown docs site, which is easy for anyone to edit without Jekyll experience.

Your root page should be `index.md` or `README.md`. There is no navbar, so it is recommended to add a menu on your homepage which links to the other pages. You can always get back to the homepage using the link added for you at the top of every page.


### Convert to Jekyll

The approach here is also flexible - you can add a `_config.yml` file and a theme to turn your site in a proper Jekyll-based themed site.

You don't even have to add metadata to your pages - the layout will be set as `default.html`.




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
