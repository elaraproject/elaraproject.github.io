# Project Elara website

This is Project Elara's website, the most up-to-date and authoritative source of information about Project Elara. This includes the latest research papers and assets and project announcements and news.

## Getting started

The site is a static site, built on [Zola](https://www.getzola.org/). To get started, download Zola, clone the git repository, enter it, and simply run:

```sh
zola serve
```

This should open a local developer server to live-reload the website.

## Developer information

The site is built on templates in the `templates/` folder. The pages themselves are in `content/` with a few exceptions (such as the research papers and other hosted assets) in the `static/` folder. Each page is markdown with some pages including a bit of HTML where it's necessary. 

Page variables are specified in YAML format like so:

```yml
+++
var1 = value1
var2 = value2
# ...
+++
```

The variables include the following:

- `title`: the name of the page, placed in double-quotes
- `date`: the date the page was first published, in `YYYY-MM-DD` format
- `description`: a short description of the page, placed in double-quotes
- Several variables placed below `[extra]`
	- `author`: for news pages only, the name of the person who wrote the article
	- `subtitle` (only on homepage): the subheader text of the front page

## Licensing info

Icons are from [boxicons](https://boxicons.com).
