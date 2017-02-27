Awesome Source CV Extended
=================

## About

**Awesome Source Latex CV** was originally based on a CV template created by Alessandro Plasmati. Thi template use _LuaLaTeX_ engine and _[Fontin Sans](http://www.exljbris.com/fontinsans.html)_ font. For Chinese support, _[Noto Sans](https://www.google.com/get/noto/) _ is applied.

***ATTENTION 1: This project can not be compiled with MiKTeX since there is unexpected errors (luelatex.exe crashed). TeXLive is highly recommended!***

***ATTENTION 2：When Chinese support is enabled, there can be a noticable increase of compiling time, please disable it if not need. 中文支持将大幅延长编译时间！***

More informations about the original Alessandro Plasmati template can be found here :

   -  [ Scribd ](http://fr.scribd.com/doc/16335667/Writing-your-Professional-CV-with-LaTeX)
   -  [ LaTeX Templates ](http://www.latextemplates.com/template/plasmati-graduate-cv)
   -  [ ShareLatex ](https://www.sharelatex.com/templates/cv-or-resume/professional-cv)

**Personal data** has moved on top of the first page just before the position and _[Fontin Sans](http://www.exljbris.com/fontinsans.html)_ font has been replaced by _[Source Sans Pro Font](https://github.com/adobe-fonts/source-sans-pro)_ from Adobe. _[Font Awesome](http://fontawesome.io/)_ icons highlight important elements.

Unlike _Alessandro Plasmati_ CV template, all layout stuff in **Awesome Source Latex CV** has moved in the Latex class file _awesome-source-cv.cls_ to imptove source code readability.

## Quick start

## How to use **Awesome Source CV** latex class

### Use the **Awesome Source CV** options

When declaring the `\documentclass` you can use option(s) to customize your CV rendering.

**Used with no option, the template will use the 'traditional' **

_header layout your system fonts and the default color scheme ie. blue_

`\documentclass{awesome-source-cv}`

**Used with localFont option the template will use the 'traditional' **

_header layout, fonts included in the fonts directory and the default color scheme_

`\documentclass[localFont]{awesome-source-cv}`

**Used with localFont option, the template will use the 'alternative' **

_header layout, your system fonts and the default color scheme_

`\documentclass[alternative]{awesome-source-cv}`

**Used with chinese option the template will support Chinese **

**使用chinese选项开启中文支持**

`\documentclass[chinese]{awesome-source-cv}`

### Construct the header

Outside of the `\socialinfo` wrapper you have to define the mandatory parameters `\name` and `\tagline`.

Most social network have their command to render a clickable link or a simple text entry.

Put these command in the `\socialinfo` wrapper. Feel free to add `\\` when you want to force a new line.

Use the `\makecvheader`command to generate the header.

Use the `\makecvheaderwithoutphoto`command to generate the header without your profile photo.

### Content sections
In every tex file of the corresponding sections, there are instructions to add entries.


## License

Latex class file _awesome-source-cv.cls_ is published under the term of the [LPPL Version 1.3c](https://www.latex-project.org/lppl.txt).

All content files are published under the term of the [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/legalcode).