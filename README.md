[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ryelaw/jekyll-serif-theme)
[![Netlify Status](https://api.netlify.com/api/v1/badges/c803b47f-87fd-4fd5-b9b6-1dfd2906ff3e/deploy-status)](https://app.netlify.com/sites/ryelawoffice/deploys)

# Ryelaw Website Source

This site is based off the `Jekyll Serif Theme and has several templates for a law office website. The theme is fully responsive, blazing fast and artfully illustrated.

- [Jekyll Serif Live Demo](https://jekyll-serif.netlify.app/) | 
- [Zerostatic Themes](https://www.zerostatic.io)

# Adding or updating Legal Services

The services pages are generated dyamically from the `_services` directory.
The files in these pages are written in a editing format called markdown.
Here's a link to a good [markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/)
for guidance on how to format the content.

Each file in `_services` will begin with a standard yaml header that tells the site generator
what the title of the page is, when it was created, whether it is featured, its ordering
weight for layout and the layout template to use.

Example Header:

```yaml
---
title: "Real Estate Transactions"  # This becomes the title of the page in H1 format.
# date: 2018-11-28T15:14:54+10:00  # This is the page creation date.  This should remain commented out.
featured: true                     # This should be set to true to feature the service on the website front page.
weight: 1                          # This controls the ordering of the content from left to right
layout: service                    # This selects the layout for the page, for services this should be service.
---
```

The remainder of the file will be the page content formatted in yaml.

# Installation

### Installing Ruby & Jekyll
 
If this is your first time using Jekyll, please follow the [Jekyll docs](https://jekyllrb.com/docs/installation/) and make sure your local environment (including Ruby) is setup correctly.

### Installing Theme

Download or clone the theme.

To run the theme locally, navigate to the theme directory and run:

```
bundle install
``` 

To start the Jekyll local development server.

```
bundle exec jekyll serve
``` 

To build the theme.
 
```
bundle exec jekyll build
```

# Deployment

## Netlify

This theme contains a `netlify.toml` and has been tested to work with Netlify.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/ryelaw/jekyll-serif-theme)

## Github Pages
This theme has been tested to work with Github Pages (and Github Project Pages)

If you are using this theme with Github Pages and you are using a Github Project Page then **your site will be hosted in a subfolder** you will need to update the `baseurl` in the `_config.yml` otherwise all the css, images and paths will be broken.

For example the site https://zerostaticthemes.github.io/jekyll-serif-theme would have `baseurl: "/jekyll-serif-theme"`


## Credits

- Beautiful royalty free Illustrations by Icons8 - https://icons8.com/illustrations/style--pixeltrue


## License

This theme is open source under the MIT license. If you fork or copy this theme you must leave me as the original author in the LICENSE file (on line 3 where I am listed as the author). Really, I just don't want people copying this theme and then saying it's their theme, because I put a lot of work into my themes, thanks!
