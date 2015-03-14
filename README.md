# CASPER theme for hugo
    

Casper is a single-column theme for [Hugo](http://gohugo.io/).

blog demo : http://vjeantet.fr

## Features

* Google Analytics (optional)
* Disqus ( can disable comments by post)
* Share buttons (Facebook, Twitter, Google)
* Big cover image (optional)
* Custom cover by post (optional)
* Tagging
* Pagination
* Menu

# Installation

## Installing this theme

    mkdir themes
    cd themes
    git clone https://github.com/vjeantet/hugo-theme-casper casper

## Build your website with this theme

    hugo server -t casper

# Configuration

**config.toml**

``` toml
BaseUrl= "http://example.com"
LanguageCode= "fr-FR"
Title= "My blog is awesome"
paginate = 5
DisqusShortname = "YOUR_SHORT_NAME_HERE"
Copyright = "All rights reserved - 2015"

[params]
  description = "this is my description"
  cover = "images/cover.jpg"
  author = "Valère JEANTET"
  logo = "images/logo.png"
  bio= "my bio"
  googleAnalyticsUserID = "UA-79101-12"
  githubName = "vjeantet"
  twitterName = "vjeantet"

```

## Menu configuration

On top right of the screen, a "Subscribe" button is displayed with a link to the RSS feed.

When you define a menu in the main config file, Then a menu button is displayed instead of the subscribe button
When the use clicks the menu button, a sidebar appears and shows the subscribe button and all items defined in the main config file

Exemple of a menu definition in main config file, 


Example : [config.toml](https://github.com/vjeantet/vjeantet.fr/blob/master/config.toml)

**example post**

``` markdown
+++
date = "2014-07-11T10:54:24+02:00"
draft = false
title = "dotScale 2014 as a sketch"
slug = "dotscale-2014-as-a-sketch"
tags = ["event","dotScale","sketchnote"]
image = "images/2014/Jul/titledotscale.png"
comments = true
+++

Contents here
```

# Create new content based with default metadata from this theme
```
hugo new -t casper post/my-post.md
```

# Contact me

open an issue in github

[https://twitter.com/vjeantet](https://twitter.com/vjeantet)
