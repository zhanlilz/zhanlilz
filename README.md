<p align="center"><a href="https://wowchemy.com" target="_blank" rel="noopener"><img src="https://wowchemy.com/img/logo_200px.png" alt="Wowchemy Website Builder"></a></p>

# Academic Template for [Hugo](https://github.com/gohugoio/hugo)

The Hugo **Academic Resumé Template** empowers you to create your job-winning online resumé and showcase your academic publications.

[Check out the latest demo](https://academic-demo.netlify.app) of what you'll get in less than 10 minutes, or [view the showcase](https://wowchemy.com/user-stories/).

[**Wowchemy**](https://wowchemy.com) makes it easy to create a beautiful website for free. Edit your site in Markdown, Jupyter, or RStudio (via Blogdown), generate it with Hugo, and deploy with GitHub or Netlify. Customize anything on your site with widgets, themes, and language packs.

- 👉 [**Get Started**](https://wowchemy.com/templates/)
- 📚 [View the **documentation**](https://wowchemy.com/docs/)
- 💬 [Chat with the **Wowchemy community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@wowchemy](https://twitter.com/wowchemy) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithWowchemy](https://twitter.com/search?q=(%23MadeWithWowchemy%20OR%20%23MadeWithAcademic)&src=typed_query)
- 💡 [Request a **feature** or report a **bug** for _Wowchemy_](https://github.com/wowchemy/wowchemy-hugo-modules/issues)
- ⬆️ **Updating Wowchemy?** View the [Update Guide](https://wowchemy.com/docs/guide/update/) and [Release Notes](https://wowchemy.com/updates/)

## Crowd-funded open-source software

To help us develop this template and software sustainably under the MIT license, we ask all individuals and businesses that use it to help support its ongoing maintenance and development via sponsorship.

### [❤️ Click here to unlock rewards with sponsorship](https://wowchemy.com/plans/)

## Ecosystem

* **[Hugo Academic CLI](https://github.com/wowchemy/hugo-academic-cli):** Automatically import publications from BibTeX

[![Screenshot](https://raw.githubusercontent.com/wowchemy/wowchemy-hugo-modules/master/academic.png)](https://wowchemy.com)

## Demo image credits

- [Open book](https://unsplash.com/photos/J4kK8b9Fgj8)
- [Course](https://unsplash.com/photos/JKUTrJ4vK00)

[![Analytics](https://ga-beacon.appspot.com/UA-78646709-2/starter-academic/readme?pixel)](https://github.com/igrigorik/ga-beacon)

## My own notes/tips on using the Academic Template

* content/publications: Add a pdf under a publication folder (e.g., li-2018)
  named after this publication folder name (i.e., li-2018.pdf under
  content/publication/li-2018). The pdf button on the publication page will give
  users the pdf.

* static/sub-folder-name: Files under this folder can be referred in the .md
  files as sub-folder-name/a-file

* menus.yaml: Change the ``weight`` property of each menu item to change its
  display location on top of the home page. The larger the weight, the more
  right / further back the item will be displayed.

* content/home/tags.md: This is the word cloud displayed under "Popular Topics"
  on the published page. It uses tags in all the .md files. Currently, most tags
  are from the index.md files in the publication folders. 

* Create a new post. For more details, https://wowchemy.com/docs/content/blog-posts/
  ```
  $ hugo new --kind post post/my-article-name
  ```

* Create a new publication. For more details, https://wowchemy.com/docs/content/publications/
  * Import from a .bib file
    ```
    $ academic import --bibtex <path_to_your/publications.bib>
    ```
  * Mannually create one
    ```
    $ hugo new --kind publication publication/<my-publication>
    ```