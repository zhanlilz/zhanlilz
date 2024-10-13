# [Hugo Academic CV Theme](https://github.com/HugoBlox/theme-academic-cv)

[![Screenshot](.github/preview.webp)](https://hugoblox.com/templates/)

The Hugo **Academic CV Template** empowers you to easily create your job-winning online resumé, showcase your academic publications, and create online courses or knowledge bases to grow your audience.

[![Get Started](https://img.shields.io/badge/-Get%20started-ff4655?style=for-the-badge)](https://hugoblox.com/templates/)
[![Discord](https://img.shields.io/discord/722225264733716590?style=for-the-badge)](https://discord.com/channels/722225264733716590/742892432458252370/742895548159492138)  
[![Twitter Follow](https://img.shields.io/twitter/follow/GetResearchDev?label=Follow%20on%20Twitter)](https://twitter.com/GetResearchDev)

️**Trusted by 250,000+ researchers, educators, and students.** Highly customizable via the integrated **no-code, Hugo Blox Builder**, making every site truly personalized ⭐⭐⭐⭐⭐

Easily write technical content with plain text Markdown, LaTeX math, diagrams, RMarkdown, or Jupyter, and import publications from BibTeX.

[Check out the latest demo](https://academic-demo.netlify.app/) of what you'll get in less than 10 minutes, or [get inspired by our academics and research groups](https://hugoblox.com/creators/).

The integrated [**Hugo Blox Builder**](https://hugoblox.com) and CMS makes it easy to create a beautiful website for free. Edit your site in the CMS (or your favorite editor), generate it with [Hugo](https://github.com/gohugoio/hugo), and deploy with GitHub or Netlify. Customize anything on your site with widgets, light/dark themes, and language packs.

- 👉 [**Get Started**](https://hugoblox.com/templates/)
- 📚 [View the **documentation**](https://docs.hugoblox.com/)
- 💬 [Chat with the **Hugo Blox Builder community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@GetResearchDev](https://twitter.com/GetResearchDev) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithHugoBlox](https://twitter.com/search?q=%23MadeWithHugoBlox&src=typed_query)
- ⬇️ **Automatically import your publications from BibTeX** with the [Hugo Academic CLI](https://github.com/GetRD/academic-file-converter)
- 💡 [Suggest an improvement](https://github.com/HugoBlox/hugo-blox-builder/issues)
- ⬆️ **Updating?** View the [Update Guide](https://docs.hugoblox.com/reference/update/) and [Release Notes](https://github.com/HugoBlox/hugo-blox-builder/releases)

## We ask you, humbly, to support this open source movement

Today we ask you to defend the open source independence of the Hugo Blox Builder and themes 🐧

We're an open source movement that depends on your support to stay online and thriving, but 99.9% of our creators don't give; they simply look the other way.

### [❤️ Click here to become a Sponsor, unlocking awesome perks such as _exclusive academic templates and blocks_](https://hugoblox.com/sponsor/)

<!--
<p align="center"><a href="https://hugoblox.com/templates/" target="_blank" rel="noopener"><img src="https://hugoblox.com/uploads/readmes/academic_logo_200px.png" alt="Hugo Academic Theme for Hugo Blox Builder"></a></p>
-->

## Demo image credits

- [Unsplash](https://unsplash.com)

## Latest news

<!--START_SECTION:news-->

- [Easily make an academic CV website to get more cites and grow your audience 🚀](https://hugoblox.com/blog/easily-make-academic-website/)
- [What&#39;s new in v5.2?](https://hugoblox.com/blog/whats-new-in-v5.2/)
- [What&#39;s new in v5.1?](https://hugoblox.com/blog/whats-new-in-v5.1/)
- [Version 5.0 (February 2021)](https://hugoblox.com/blog/version-5.0-february-2021/)
- [Version 5.0 Beta 3 (February 2021)](https://hugoblox.com/blog/version-5.0-beta-3-february-2021/)
<!--END_SECTION:news-->

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
6. Update the Wowchemy website components that my website uses, refer to https://wowchemy.com/docs/hugo-tutorials/update/

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

* Disable/Enable a widget (or visually a section on my website)
For example, to disable the section **Post**, 
  * go to `content/home/posts.md`, look for the following two lines
    ```md
    # Activate this widget? true/false
    active: false
    ```  
    If `active: false`, the widget/section will not show on the website. If `active: true`, it will show. 
  * Do NOT forget to edit `config/_default/menus.yaml` to remove this section
  from the top menu if it was an item on the menu.
