---
title: Wondrous Isles Data
layout: page
---

## Visualize

- [Word cloud]({{ '/data/cloud.html' | absolute_url }})
- [Word Tree](https://www.jasondavies.com/wordtree/?source=https%3A%2F%2Fevanwill.github.io%2Fmorris-wondrous-isles-book%2Fdata%2Fmorris_wondrous-isles_1897.txt){:target='_blank'} (jasondavies)

## Text Download

*derivatives generated from the project text.*

- HTML full text: [morris_wondrous-isles_1897.html]({{ '/data/morris_wondrous-isles_1897.html' | absolute_url }}){:target='_blank'} (*minimal html with full text content*)
- Plain text: [morris_wondrous-isles_1897.txt]({{ '/data/morris_wondrous-isles_1897.txt' | absolute_url }}){:target='_blank'}
- Minimized plain text: [morris_wondrous-isles_1897_min.txt]({{ '/data/morris_wondrous-isles_1897_min.txt' | absolute_url }}){:target='_blank'} (*no front matter, no chapter names, no line breaks except between chapters*)
- CSV: [morris_wondrous-isles_1897.csv]({{ '/data/morris_wondrous-isles_1897.csv' | absolute_url }}){:target='_blank'} (*each chapter is a row, with columns chapter_number, chapter_title, chapter_text*)
- Mallet: [mallet.txt]({{ '/data/mallet.txt' | absolute_url }}){:target='_blank'} (*each paragraph is a "document" in the standard Mallet tab delimited format: ID tab label tab text. This file is ready for upload to [jsLDA](https://mimno.infosci.cornell.edu/jsLDA/)*)

## Metadata

{% include utilities/get_full_text.html %}
{%- include utilities/remove_punctuation.html -%}
{%- assign full_text = full_text | downcase | normalize_whitespace -%}
{%- assign word_count = full_text | number_of_words -%}
{%- assign unique_words = full_text | split: " " | uniq | size -%}
{%- assign character_count = full_text | size -%}

*calculated from text excluding front matter and chapter headings.*

- Total words count: {{ word_count }}
- Unique words: {{ unique_words }} (download [words.csv]({{ '/data/words.csv' | absolute_url }}){:target='_blank'})
- Vocabulary density: {% assign w_float = word_count | times: 1.0 %}{{ unique_words | divided_by: w_float | round: 4 }}
- Character count: {{ character_count }} (download unique [characters.csv]({{ '/data/characters.csv' | absolute_url }}){:target='_blank'})
- Line count: 477 (approximately paragraphs)
- Chapter word counts: [wordcounts.csv]({{ '/data/wordcounts.csv' | absolute_url }}{:target='_blank'})

## Source Texts

- [Kelmscott Press, 1897, Cleveland Museum of Art](https://archive.org/details/MorrisWaterWondrousIsles).
- [Longmans, Green, and Co., 1897, Trent University](https://archive.org/details/waterofwondrousi0000morr) (not particularly good digitization).
- Longmans, Green, and Co.,"Pocket edition", 1914, [Vol. I](https://archive.org/details/waterofwondrousi01morruoft), [Vol. II](https://archive.org/details/waterofwondrousi02morruoft), University of Toronto.
- [William Morris Archive, edited by Florence S. Boos](http://morrisedition.lib.uiowa.edu/waterwondrousisles.html) (good text, but dated html template and non-working page image editions)

## Source Code

- [morris-wondrous-isles-book]({{ site.github-repo }}) (on GitHub)
