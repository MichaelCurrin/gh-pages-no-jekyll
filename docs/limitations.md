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

Links to markdown files have to be done differently. See below. If there are broken internal links, the build will fail.

```md
- [Foo](foo)
```

Note on the extension of targets:

- Note no extension. The `.md` file is actually there too on the remote server, but if you try and enter it in the URL you'll get prompted to download it.
- Note no leading forwardlash - this allows your site to serve on a GitHub Pages subpath.
- That points to `/foo` (no extension or trailing slash), which is an alias for `/foo.html`.

### Debugging

Github Pages error messages on a build on a limited.

And you probably need to install something to test the build locally.

### Badges

If you try and use a shields.io badge inside a centered badge, the code will get shown as plain text. This is an issue on a normal Jekyll site.

So take out the centering, or use HTML instead of markdown.
