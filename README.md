# SyRF User Guide

Before editing the user guide, please read the instructions below.

## Theme

This repository uses the [just-the-docs](https://github.com/just-the-docs/just-the-docs) remote theme.

## Editing the `_config.yml` file

Familiarise yourself with the [just-the-docs config file](https://github.com/just-the-docs/just-the-docs/blob/main/_config.yml) before attempting to edit this file, as incorrect changes may cause the site build to fail.

## Adding a new page

To add a new file, click `add file` and `create new file` at the top of the GitHub repository. Name the file something sensible and add `.md` to the end of the file name.

Make sure to add the following to the top of the file:

```
---
title: My Page Title
parent: Title of the Parent Page
has_children: false
nav_order: 1
layout: page
---
```

- `title`: the title of your page
- `parent`: the title of the parent page. If your page is not a child page, delete this row
- `has_children`: true or false. Select true if your page has child pages
- `nav_order`: a number which reflects the order the page appears in the side navigation bar. 1 is first, 2 is second, etc...

Once you have this, you can add the page content below. Finally, click `commit` when you are done. GitHub will build your page and in a few minutes it will appear on the live site.

## Editing a page

You can edit pages directly in GitHub. After your commit our changes, it will take a few minutes to see them on the live site.

## Adding an image

First add your image to the `figs` folder. Next, open the page where you want the image to dosplay and add the following line of code:

```
![alt text for the image](figs/my_image_file_name.png)
```
Make sure to add alternative text (for screen readers) and the correct name of the file you want to display.
