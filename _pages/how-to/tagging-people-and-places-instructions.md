---
layout: page
title: Tagging people and places
permalink: /how-to/tagging-people-and-places-instructions/
author: Will Hanley
header:
  image_fullwidth: masthead.jpg
---
## Objectives

The greatest use for the encoded *Egyptian Gazette* will come in linking its content to other data sets. There are wonderful datasets listing people and places of the past.  This tutorial explains how we will link our project to those projects. To do so, we will use the Text Encoding Initiative (TEI)'s [rich schema for tagging people and places](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ND.html).

## Tagging places
The basic tag that we will use is `<placeName>`. Full details of usage are [here](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ND.html#NDPLAC) and  [here](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ref-placeName.html).

The key element we will use to link our places to other date sets is `ref=`. We can use this to link to authorities such as wikidata, geonames, or [geohack](https://tools.wmflabs.org/geohack/geohack.php?pagename=Alexandria&params=31_12_N_29_55_E_type:city(4546231)_region:EG).
