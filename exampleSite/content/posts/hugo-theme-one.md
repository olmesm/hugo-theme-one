---
title: "Hugo Theme One"
date: 2017-12-20T04:22:12+08:00
tags: ["hugo","theme"]
draft: false
---

[One](https://github.com/resugary/hugo-theme-one) is a minimal blog theme for Hugo, which is forked from [onetwothree](https://github.com/schollz/onetwothree). 

## Differences from onetwothree

It provides some new features and simplifications. I tried to keep it minimal with less configuration to write and express yourself rather than play with a theme instead.

Features:  
- Add archives support for all blog posts in a single page  
- Homepage posts customizable, default with 7 latest posts instead of all posts  
- Sytax highlighting with `highlight.js`  
- Google Analytics support  
- Full-text RSS support

Some simplifications:  
- Remove the style "2" and "3" in adittion  
- Remove PREVIOUS and NEXT links at bottom of posts  
- Remove twitter components integrated
- Remove rounded edges style of images    
- Remove tags displayed following each titles at homepage  
- Change preformatted style of code block and blockquote  
- Change posts location to `content/posts` as [hugo Quick Start](https://gohugo.io/getting-started/quick-start/) 

## Installation

Clone this repository to your hugo theme directory.

```
git clone https://github.com/resugary/hugo-theme-one.git themes/one
hugo server -t=one
```


## Create New Posts

Posts should generally go under a `content/posts` directory, you may start like this:

```
hugo new posts/hello.md
```

## Create a fixed Page

Fixed pages such as an About page should be present at the root of the `content` directory:

```
hugo new about.md
```

To enable Archives, you should create a new file called `archives.md`:

```
hugo new archives.md

# then add the following line in the front matter
type: "archives"
```

## Configuration

Copy the `config.toml` in the root director of your hugo site. 

```toml
baseURL = "https://example.com"
languageCode = "en-us"
title = "My Hugo Site"

theme = "one"
googleAnalytics = "UA-123-45"

[params]
    navigation = ["archives.md", "about.md"]

```

Feel free to change the strings in this theme.

## License

Licensed under the MIT License. See the [LICENSE](https://github.com/resugary/hugo-theme-one/blob/master/LICENSE.md) file for more details.