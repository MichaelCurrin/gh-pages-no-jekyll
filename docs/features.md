# **Features**

- Suitable for light docs site of a few pages.
- No HTML or Liquid coding needed. Just write content in markdown.
- No coding experience need to setup or work on.
- No Jekyll config, theme or packages to install.
- Uses a default minimal theme provided by GitHub - this is similar to viewing pages on GitHub itself but is cleaner on the edges.
- The build will add a homepage link to the top of each page. That is `h1`, so you first heading on the page should be an `h2`.
- There's an _Improve this page_ button in the bottom right of eac hpage.
- This pattern for a GH Pages site works using content in your `docs` directory. But you can also move everything to the root, such as if the entire repo is documentation, or if you are making a website that is not about documetnation. Just configure GH Pages to use the appropriate path.


## Styling

Example code block:

```sh
echo 'Hello, world!'
```

Remember to use `h2` elements at the top of your page, as `h1` is already taken care of as a header.

e.g.

```md
## About

Content here.
```


## Jekyll vs no Jekyll

### No Jekyll

If you want to upload plain HTML instead of `.md` files, create an empty `.nojekyll` file in your repo.

### Jekyll

If you want to upload markdown and have it rendered to HTML with Github's base styling, leave the `.nojekyll` file out so that Jekyll is used. Note that you don't need any config, Gemfile, theme etc. Just an `index.md` page and optionally more linked pages will work.

Jekyll will turn `index.md` into `index.html`. Any Liquid code for Jekyll can cause build errors, so since you're using Jekyll to parse you files you should use the `raw` tag to prevent the Liquid from being evaluated and rather render as plain text (typically in a codeblock).


## Homepage

The homepage needs be available as `/` i.e. `/index.html` when the site is rendered.

Therefore your homepage should be named `index.md`.

Or, name it `README.md` and use the following Jekyll frontmatter:

```liquid
---
permalink: /
---
# **Documentation**
```


## Navigation

Internall links to pages can be one of these.

```md
[Alt text](foo.md)
```

Which points to `/foo.html`.

Or this.

```md
[Alt text](foo)
```

Which points to `/foo`.

Remember to omit the leading slash in your path, otherwise you'll break links on a subpath project site on GH Pages.

If there are broken internal links, the build will fail, which is useful.
