Awesome Source CV [![Example](https://img.shields.io/badge/Exemple-pdf-blue.svg)](https://github.com/darwiin/awesome-neue-latex-cv/releases/download/1.4-github/cv.pdf)
=================

## About

**Awesome Source Latex CV** was originally based on a CV template created by Alessandro Plasmati. Thi template use _XeLaTeX_ engine and _[Fontin Sans](http://www.exljbris.com/fontinsans.html)_ font. 

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

```latex
% Used with no option, the template will use the 'traditional' 
% header layout your system fonts and the default color scheme ie. blue
\documentclass{awesome-source-cv}

% Used with localFont option the template will use the 'traditional' 
% header layout, fonts included in the fonts directory and the default color scheme
\documentclass[localFont]{awesome-source-cv}

% Used with chinese option the template will support Chinese 
% header layout, fonts included in the fonts directory and the default color scheme
\documentclass[chinese]{awesome-source-cv}

=================

## About

**Awesome Source Latex CV** was originally based on a CV template created by Alessandro Plasmati. Thi template use _XeLaTeX_ engine and _[Fontin Sans](http://www.exljbris.com/fontinsans.html)_ font. 


**Personal data** has moved on top of the first page just before the position and _[Fontin Sans](http://www.exljbris.com/fontinsans.html)_ font has been replaced by _[Source Sans Pro Font](https://github.com/adobe-fonts/source-sans-pro)_ from Adobe. _[Font Awesome](http://fontawesome.io/)_ icons highlight important elements.

Unlike _Alessandro Plasmati_ CV template, all layout stuff in **Awesome Source Latex CV** has moved in the Latex class file _awesome-source-cv.cls_ to imptove source code readability.

## How to use **Awesome Source CV** latex class

### Use the **Awesome Source CV** options

When declaring the `\documentclass` you can use option(s) to customize your CV rendering.

```latex
% Used with no option, the template will use the 'traditional' 
% header layout your system fonts and the default color scheme ie. blue
\documentclass{awesome-source-cv}

% Used with localFont option the template will use the 'traditional' 
% header layout, fonts included in the fonts directory and the default color scheme
\documentclass[localFont]{awesome-source-cv}

% Used with localFont option, the template will use the 'alternative' 
% header layout, your system fonts and the default color scheme
\documentclass[alternative]{awesome-source-cv}

% Used with chinese option the template will support Chinese 
% header layout, fonts included in the fonts directory and the default color scheme
\documentclass[chinese]{awesome-source-cv}

```

### Construct the header

Outside of the `\socialinfo` wrapper you have to define the mandatory parameters `\name` and `\tagline`.

```latex
% Define author's name
% Usage: \name{<firstname>}{<lastname>}
% Mandatory
\name{Christophe}{ROGER}

% Define author's photo (optional)
% Usage \photo{<diameter>}{<photo>}
\photo{2.5cm}{darwiin}

% Define author's tagline
% Usage: \tagline{<tag line>} 
% Mandatory
\tagline{Chef de projet IT}
```

Most social network have their command to render a clickable link or a simple text entry.

```latex
% Render author's linked-in (optional)
% Usage: \linkedin{<linked-in-nick>}
\linkedin{christopheroger}

% Render author's viadeo(optional)
% Usage: \viadeo{<viadeo-nick>}
\viadeo{christopheroger}

% Render author's github (optional)
% Usage: \github{<github-nick>}
\github{darwiin}

% Render author's email (optional)
% Usage: \email{<email adress>}
\email{christophe.roger@mail.com}
```

Put these command in the `\socialinfo` wrapper. Feel free to add `\\` when you want to force a new line.

```latex
\socialinfo{
  \linkedin{christopheroger}
  \viadeo{christopheroger}
  \github{darwiin}\\
  \smartphone{+687 123 456}
  \email{christophe.roger@mail.com}\\
  \address{2 Rue du quartier, 98765 Ville, Pays}\\
  \infos{Né le 23 septembre 1982 (34 ans) à Nouméa, Nouvelle-Calédonie}
}
```

Use the `\makecvheader`command to generate the header.

Use the `\makecvheaderwithoutphoto`command to generate the header without your profile photo.

```latex
\makecvheader
```

```latex
\makecvheaderwithoutphoto
```


## License

Latex class file _awesome-source-cv.cls_ is published under the term of the [LPPL Version 1.3c](https://www.latex-project.org/lppl.txt).

All content files are published under the term of the [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/legalcode).
