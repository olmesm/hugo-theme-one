One
===========

[One](https://github.com/resugary/hugo-theme-one) is a mininal blog theme for [Hugo](https://gohugo.io/), which is forked from [onetwothree](https://github.com/schollz/onetwothree). It provides some new features and simplification. I tried to keep it simple with less configuration to write rather than play with a theme instead.

You can check out the demo at https://resugary.github.io/hugo-theme-one.

![Screenshot](https://github.com/resugary/hugo-theme-one/blob/master/images/screenshot.png)

Features:  
- Add posts archive support  
- Add syntax highlighting using Chroma  
- Add Google Analytics support  
- Add Full-text RSS support

## Installation

Clone this repository to your hugo theme directory:

```
git clone --depth=1 https://github.com/resugary/hugo-theme-one.git themes/one
```

## Create New Posts

Posts should generally go under the `content/posts` directory, you may start like this:

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

# then add the following line in the front matter of archives.md
type: "archives"
```

Take a look inside the [exampleSite](https://github.com/resugary/hugo-theme-one/tree/master/exampleSite) folder if you get stuck.

## Configuration

Copy the `config.toml` in the root director of your hugo site. 

```toml
# End your baseURL with a `/` trailing slash, e.g. `https://example.com/`.
baseURL = "https://example.com/"

languageCode = "en-us"
title = "My Hugo Site"
theme = "one"
googleAnalytics = "UA-123-45"

# Chroma syntax highlighting
pygmentsCodefences = true
pygmentsCodefencesGuessSyntax = true
pygmentsStyle = "pygments"

# Custom navigation bar
[params]
    navigation = ["archives.md", "about.md"]

```

## License

Licensed under the MIT License.
