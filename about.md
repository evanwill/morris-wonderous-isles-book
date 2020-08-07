---
title: About wondrous-isles-book
layout: page
---

*The Water of the Wondrous Isles* is a classic fantasy novel by [William Morris](https://en.wikipedia.org/wiki/William_Morris), first published in 1897 as an elaborate artisanal vellum print edition produced at [Kelmscott Press](https://en.wikipedia.org/wiki/Kelmscott_Press).

`morris-wondrous-isles-book` is an *artisanal* web based digital edition.

Other digitized editions:

- [Kelmscott Press, 1897, Cleveland Museum of Art](https://archive.org/details/MorrisWaterWondrousIsles).
- [Longmans, Green, and Co., 1897, Trent University](https://archive.org/details/waterofwondrousi0000morr) (not particularly good digitization).
- Longmans, Green, and Co.,"Pocket edition", 1914, [Vol. I](https://archive.org/details/waterofwondrousi01morruoft), [Vol. II](https://archive.org/details/waterofwondrousi02morruoft), University of Toronto.
- [William Morris Archive, edited by Florence S. Boos](http://morrisedition.lib.uiowa.edu/waterwondrousisles.html) (good text, but dated html template and non-working page image editions)

## Technical 

The site was developed from the [basic-book](https://github.com/evanwill/basic-book) template, using [Jekyll](http://jekyllrb.com/) static site generator and hosted on [GitHub Pages](https://pages.github.com/).
This version uses Jekyll 4.0.1 and a custom plugin, and is built using GitHub Actions.

The text is stored as a series of plain text files in Markdown format, one for each chapter.
This text is used to generate both the web pages of the book and [data derivatives]({{ '/data/' | absolute_url }}) for importing into other tools for analysis.

The source code is hosted in a GitHub repository, [morris-wondrous-isles-book]({{ site.github-repo }}).
This allows the book to be easily shared, adapted, and modified by anyone--or used as a template for creating other books.

## License 

The text of Wondrous Isles was originally published in 1897 in the UK, thus is in the Public Domain.
The website project is [licensed MIT (copyright Evan Will)](https://github.com/evanwill/morris-wondrous-isles-book/blob/master/LICENSE), and other content are <a href="https://creativecommons.org/licenses/by-sa/4.0/" target="_blank" >CC BY-SA</a> by [Evan Will](https://github.com/evanwill), {{ site.site-date }}.
