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

```
- [Foo](foo)
```

Note on the extension of targets:

- Note **lack** of `.md` in path for the docs site to work. The `.md` file is actually there too on the remote server, but if you try and enter it in the URL you'll get prompted to download it.
- If you look at a file like on Github such as `https://github.com/USERNAME/REPO/docs/index.md`, if you click the link to Foo you'll get a page with a URL ending with `/foo`. This will appear as an error but this is fine.

### Debugging

Github Pages error messages on a build on a limited.

And you probably need to install something to test the build locally.
