## About

This project is a built around GitHub's functionality which lets you use GitHub Pages to render markdown (or HTML) files as a static website, from your root or `docs` folder. 

Jekyll is still actually used to convert the files, but the project works with **no** typical Jekyll files such as layouts, themes, gems or configs. Github handles the CSS styling with a basic blue and white theme.

This means it is very **light**, as you only write content.

Note you can still use Jekyll Liquid templating. But the idea for this project is to avoid it and make a plain markdown docs site, which is easy for anyone to edit without Jekyll experience.

Your root page should be `index.md` or `README.md`. There is no navbar, so it is recommended to add a menu on your homepage which links to the other pages. You can always get back to the homepage using the link added for you at the top of every page.
