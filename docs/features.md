## Features

- Use built in styling - CSS added for centered layout which is cleaner than a plain view of markdown files in a repo. 
- Build will at a homepage link to the top of each page. That is `h1`, so you first heading on the page should be an `h2`.
- There's an improve this page button the bottom right.
- Serve from project root or `docs` directory - like a Jekyll site.


### Styling

Example code block:

```sh
echo 'Hello, world!'
```

### Jekyll vs no Jekyll

#### No Jekyll

If you want to upload plain HTML instead of `.md` files, create an empty `.nojekyll` file in your repo.

#### Jekyll

If you want to upload markdown and have it rendered to HTML with Github's base styling, leave the `.nojekyll` file out so that Jekyll is used. Note that you don't need any config, Gemfile, theme etc. Just an `index.md` page and optionally more linked pages will work.


Jekyll will turn `index.md` into `index.html`. Any Liquid code for Jekyll can cause build errors, so since you're using Jekyll to parse you files you should use the `raw` tag to prevent the Liquid from being evaluated and rather render as plain text (typically in a codeblock). 


### Links

Links will have to be to `[link label](page)` and not to `[link label](page.md)`.

Keep your URLs relative so that your project title can prefixed for you. 

e.g.

- `page` will become `/my-project/page.html` 
- `/page` will become `/page.html` and be a broken link.
