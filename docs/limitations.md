# **Limitations**

## Debugging

GitHub Pages error messages on a build are limited.

There is no flow for setting up this project locally, which also makes debugging harder. You could install and run Jekyll though if you need to.


## Badges

If you try and use a _shields.io_ badge inside a centered badge, the code will get shown as plain text. This is an issue on a normal Jekyll site.

So take out the centering, or use HTML instead of markdown.


## No templating

The menus are all maintained by hand. This great for a docs site of a handful of pages. But if you site gets bigger, you should consider using Jekyll or MkDocs or DocsifyJS instead.

Those are also good options if you want a themed site, rather than the plain white layout with no navbar.


## Headings

The GitHub-styled site already has an H1 link at the top of the pages, which takes you to the site's homepage.

So when you write a heading for a page, it looks funny to do as simple H1 heading under it.

Using H1 and bold looks better. That is not great for accessibility though to have two H1s. The first is kind of a logo though and not really the page's heading.

Or your first custom heading on a page can be H2. It just means everything on the page needs to have additional header level added.
