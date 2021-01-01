## Features

- A very light website site - no Jekyll config or theme or gems.
- Uses built-in styling provided by GitHub Pages - this is similar to viewing pages on GitHub but is cleaner.
- The build will add a homepage link to the top of each page. That is `h1`, so you first heading on the page should be an `h2`.
- There's an _Improve this page_ button  inthe bottom right.
- Setup your project around your project root, or your `docs` directory for a docs site.

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
