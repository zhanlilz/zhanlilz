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

## My own notes on quick start on a new Ubuntu computer
1. Install Hugo
    * Download hugo_**extended**_VERSION_Linux-64bit.deb from https://github.com/gohugoio/hugo/releases. Note that you have to get the **extended** version for the website based on Wowchemy template to work. 
    * Double click the .deb to install Hugo. 
2. Install Hugo's Go dependency, in a terminal
```bash
sudo snap install --classic go
```
3. Install the [Hugo Academic CLI](https://github.com/wowchemy/hugo-academic-cli), in a terminal
```bash
pip3 install -U academic
```
4. Clone the repository from my Github, in a terminal 
```bash
git clone git@github.com:zhanlilz/zhanlilz.github.io.git
```
There are three branches, 
* Branch `master`: where I work on my website. Any changes made here are not deployed on my actual personal website. I should preview changes here using the script `view.sh` in the top directory.
* Branch `ready`: where I merge proofed changes from the branch `master`. Any changes made here will trigger a [Github workflow](https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions) called `gh-pages.yml` that is saved under `.github/workflows/`. This workflow will generate the actual website files (all the HTML, CSS and such) and save/update them on the branch `gh-pages`.
* Branch `gh-pages`: where the actual website files are stored and served by the Github Pages online under the URL of my personal webpage, https://zhanlilz.github.io/
5. Preview the website, ini a terminal
```bash
# In the top directory of the website repository
./view.sh
```

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

* Highlight an author name.
  * Edit the file `content/authors/<first_name>-<last_name>/_index.md`. In
  the front matter of the .md file, add/change `highlight_name: true`. If the
  author name in the index.md file of a publication appears as "first_name
  last_name", then this author name will be automatically recognized as the
  author in the folder `content/authors/<first_name>-<last_name>`. Otherwise,
  you need to use `<first_name>-<last_name>` in the index.md file of a
  publication.
  * Tip: according to https://wowchemy.com/docs/getting-started/get-started/,
  usernames (names of the folders under `content/authors/`) must be lowercase
  with any spaces replaced with hyphens (-).