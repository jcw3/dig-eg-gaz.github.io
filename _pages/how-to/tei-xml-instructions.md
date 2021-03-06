---
layout: page
title: TEI-XML instructions
permalink: /how-to/tei-xml-instructions/
author: Will Hanley
header:
  image_fullwidth: masthead.jpg
---

## Objective
These instructions guide you in transforming your plain text page files into a marked-up xml document that conforms to the standards of [TEI](http://www.tei-c.org) (the Text Encoding Initiative).

## 1. Set up your XML editor
Download the full-function Oxygen XML Editor, which offers a [free 30-day trial](http://www.oxygenxml.com/xml_editor/register.html).

## 2. Create an xml file
Copy and paste [this template](https://raw.githubusercontent.com/dig-eg-gaz/boilerplates/master/empty-issue.xml) into a new document. Name this document using the date of the issue and an xml extension (YYYY-MM-DD.xml). (This document will eventually contain all of the pages of the issue, so it is not necessary to add the page number to the document name.) Save this document on your hard drive.

## 3. Fill in the header and paste in a page of text
Enter your name into the template (under `<editor>`), today's date (under `<edition>`, in text and numeric formats), and the issue date (under `<bibl>`, in text and numeric formats). Save your file. Open a page 3 text file that you've corrected, and copy the contents. Return to the xml file and locate the `<div type="page" n="3"> </div>` pair of tags. Paste page 3 text in between these tags. Atom will immediately tell you that you have many errors and issues. Don't fret--we'll address them in the next step. Save the file.

## 4. Add structural tags
Wrap the text in tags. For now, we'll limit ourselves to three tags:
-  `<div type="item">`, which you can use for articles, items, or any division of the page that makes sense to you,
- `<head>`, which indicates a headline,
- `<p>`, which indicates a paragraph.

Oxygen offers many shortcuts to make this work go faster. Highlight the text you wish to wrap, then hit `command-E`. You will be offered a menu of tags. Choose the one you want. If you want to add more tags of the same type, hit `command-slash`.

## 5. Fork the organization content repository and save to GitHub

Once you've completed some of the structural tagging of your page, it's time to save it to GitHub. We're going to use the "fork" and "pull" functions of GitHub to do this. First, "**fork**" the [dig-eg-gaz/content](https://github.com/dig-eg-gaz/content) repository by clicking on the "fork" icon on the top right. You will be offered the chance to fork the repository under your own username--do so. This will make a copy of the repository in your own GitHub account, in which you should save your .xml page files. Later, when your page files are complete, you can fold them back into the organization content repository by sending me a **pull request**. You do this by clicking the "new pull request" button the top left above your list of files. I will then see the pull request and either merge your files into the organization's content or request that you change something before doing so.

## 6. Add more complex tags
There are more tags that you can add:
- `<cb/>` for column breaks
- `<div type="section">` to wrap multiple items
- `<dateline>` for datelines
- `<byline>` for authors
