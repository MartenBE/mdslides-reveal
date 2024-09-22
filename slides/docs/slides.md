---
title: "Would you like to know more?"
---

# MkSlides

Created by [MartenBE](https://github.com/MartenBE)

Hosted on [GitHub](https://github.com/MartenBE/mkslides) and [PyPI](https://pypi.org/project/mkslides/)

Inspired by [MkDocs](https://pypi.org/project/mkdocs/) and [reveal-md](https://github.com/webpro/reveal-md)

---

## What does it do?

<img src="./img/markdown-logo.png" height="100px" style="margin-right: 50px;"/>
<img src="./img/reveal-js-logo.svg" height="100px"/>

-   Build static HTML slideshow files from Markdown files.
    -   Turn a single Markdown file into a HTML slideshow.
    -   Turn a folder with Markdown files into a collection of HTML slideshows.
-   Publish your slideshow(s) anywhere that static files can be served.
    -   Locally, on a webserver, deploy through CI/CD with GitHub/GitLab (like this repo!), ...

---

-   Preview your site as you work, thanks to [python-livereload](https://pypi.org/project/livereload/).
-   Use custom favicons, CSS themes, templates, ... if desired.
-   Support for emojis :smile: :tada: :rocket: :sparkles: thanks to [emoji](https://github.com/carpedm20/emoji/)
-   Depends heavily on integration/unit tests to prevent regressions.
-   And more!

---

## Installation

```console
$ pip install mkslides
```

---

## Usage

-   Input
    -   Markdown **file**
    -   or **directory** with multiple (nested) Markdown files
        - This will also generate an index page like [this](./index.html)
-   Output
    -   Folder with static HTML slides
        -   Includes an index.html page with links to each slideshow when the input was a directory
-   Can be used for
    -   Local slides
    -   Hosted slides on webserver
    -   Slides generated automatically by CI/CD using Markdown files in GitHub/GitLab repo
        -   That's exactly what is happening [here](https://github.com/MartenBE/mkslides/blob/main/.github/workflows/publish.yml)!

---

## CLI

-   Generate the static HTML files

    -   from a directory:

        ```bash
        mkslides build docs/
        ```

    -   Or from just a file

        ```bash
        mkslides build docs/slides.md
        ```

---

## CLI

-   Live preview:

    -   from a directory:

        ```bash
        mkslides serve docs/
        ```

    -   Or from just a file

        ```bash
        mkslides serve docs/slides.md
        ```

---

## Customizable

-   Configuration in `mkslides.yml`
-   You can customize:
    -   Index page:
        -   Theme (local file or by public URL)
        -   Favicon (local file or by public URL)
        -   Title
        -   Template for the output HTML page
    -   Slides
        -   Theme (local file, [Reveal.js theme](https://revealjs.com/themes/), or by public URL)
        -   Highlight.js Theme (local file, [highlight.js theme](https://highlightjs.org/examples), or by public URL)
        -   Favicon (local file or by public URL)
        -   Title
        -   Template for the output HTML page

---

## Example

<iframe width="1280" height="720" src="https://www.youtube.com/embed/D9RSATHFf7U?si=Jr7Nj5Y8vaDzU_R6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Contributions

-   MkSlides is and always will be open source
    -   [MIT license](https://github.com/MartenBE/mkslides/blob/main/LICENSE)
-   Contributions are very welcome!
    -   Open an issue and/or PR
    -   We only ask that you try real hard to include **tests**!
        -   Almost everything is [tested automatically](https://github.com/MartenBE/mkslides/tree/main/tests)

---

## Example

-   This slideshow
-   [Slides](https://hogenttin.github.io/hogent-markdown-slides/) with all possibilities using Reveal.js using the [HOGENT](https://hogent.be/) theme.
    -   Also includes a lot of advanced examples such as [Mermaid.js](https://mermaid.js.org/) and [PlantUML](https://plantuml.com/) support, multicolumn slides, CI/CD, ... .
    -   Markdown can be found [here](https://github.com/HoGentTIN/hogent-markdown-slides).

---
