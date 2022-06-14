# Static site builder
A simple static site builder build on markdown files.

## Requirements
To run this site builder you need node.js installed

## Initial site setup


Clone the generator files as a submodule:
`git clone https://github.com/knaw-huc/static-site-generator.git`
`git submodule init`
`git submodule update`

`cd static-site-generator`
`npm install`

`npm run init`
`npm run start`

## Site setup
After the initial site setup,a folder is placed claas `content`. This folder contains three subfolders: _data_, _images_ and _markdown_. You can ignore the _data_ folder. All the images are stored in the _images_ folder.
The markdown files are stored in the folder _markdown_.

## Languages
You can have multiple languages for your site. For each language add a folder in the _markdown_ folder named with a language code. For example: `en` for English, `nl`for Dutch. By default an `en` folder is created.

## Site structure
The structure or site tree of your site is filed in the naming of the markdown files. The first 5 characters of the filename set the structure. The first 2 digits set the top level. The two digits after the underscore set the second level pages. A top level page has 00 as a second level. The homepage always starts with 00_00. After the first five digets you enter a name of the flie. Here's an example:

```
00_00_home.md
01_00_about.md
01_01_information.md
01_02_colofon.md
02_00_contact.md
```

These files create a site with the following site structure:
```
Home
About
- Information
- Colofon
Contact
```







## metadata
title: Tekstanalyse
author: Arno Bosse
type: news / feature / page
list_feature: true // feature list
list_news: true // news list
list_subpages: true // underlaying pages (level 2)
publication_date: 22-03-2022
summary: // teaser text for news snippits
meta_description:
meta_keyword:
featured_image: // thumbnail for overview page. Image for sharing
directSubpages: true // dont show the page content but the first child
