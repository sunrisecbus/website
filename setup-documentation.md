# Setup Documentation

This will document how the Hugo website is setup. 
This does *not* cover adding content to the site - that is in the documentation package. 
This document assumes a higher degree of technical knowledge than that document.

## Layout Files

Per [How do I use hugo without a theme](https://discourse.gohugo.io/t/how-do-i-use-hugo-without-a-theme/41243) and the Hugo [Template lookup order](https://gohugo.io/templates/lookup-order/) we need two layout files in these paths: `_default/single.html` (fo single pages like posts) and `_default/list.html` for list pages like the Home page.

We could also do the Home page as raw HTML - that's what I'm used to doing. But, we want everyone in Sunrise to be able to edit the pages, including the home page. So we want everything as simple Markdown. 

So, instead we will utilize the "base template for home page". This allows me to put the HTML stuff in the template (such as the header), and then everyone else can edit the content of the Markdown for the copywriting.

### baseof.html

This file runs on every single page no matter what. So, it has everything all pages need. The title is set, links are setup, the charset, and so on. 
