## Limitations

### Homepage

The homepage needs be available as `/` i.e. `/index.html` when the site is rendered. 

Therefore your homepage should be named `index.md`. 

Or, name it `README.md` and use the following Jekyll frontmatter:

```
---
permalink:
---
# Documentation
```

### Navigation

If there are broken internal links, the build will fail.

```md
- [Foo](foo)
```

That points to `/foo` (no extension or trailing slash), which is an alias for `/foo.html`.

Or you can use:

```md
- [Foo](foo.md)
```

Which will point to `/foo.html`.

Note no leading forward slash in paths - this allows your site to serve on a GitHub Pages subpath.

### Debugging

Github Pages error messages on a build are limited.

There is no flow for setting up this project locally, which also makes debugging harder. You could install and run Jekyll though if you need to.

### Badges

If you try and use a shields.io badge inside a centered badge, the code will get shown as plain text. This is an issue on a normal Jekyll site.

So take out the centering, or use HTML instead of markdown.
