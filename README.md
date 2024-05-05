# Teko - Hugo theme
Teko is a minimal and clean theme for hugo with a markdown-ish UI.

Forked from [Archie Theme](https://github.com/athul/archie)

## Demo

[Check the Demo](https://athul.github.io/Teko/) hosted on GitHub Pages :smile: . You can find the source code to that in the `site` branch of this repository

![](/images/theme.png)
![](/images/Teko-dark.png)
## Feature
- Google Analytics Script
- Callouts
- Tags
- Auto Dark Mode(based on system theme)
- Dark/Light Mode toggle
- tl:dr; frontamatter
- Cache busting for CSS files
- Disqus Comments

## Installation
In your Hugo website directory, create a new folder named theme and clone the repo
```bash
$ mkdir themes
$ cd themes
$ git clone https://github.com/duarte2025/teko.git
```
Edit the `config.toml` file with `theme="Teko"`
For more information read the official [setup guide](https://gohugo.io/installation/) of Hugo.

If you encounter any issues with Google Analytics, update Hugo to v0.125.0 or
later and make sure your using the latest version of the theme.

## Writing Posts
Create a new `.md` file in the *content/posts* folder
```yml
---
title: Title of the post
description:
date:
tldr: (optional)
draft: true/false (optional)
tags: [tag names] (optional)
---
```

## Credits
Forked from [Archie Theme](https://github.com/athul/archie) and Licensed under MIT License
Inspired by design of blog.jse.li

----

## Config Options

### Custom CSS
Custom CSS files can be included though the `customcss` config parameter.

Note: CSS files should be placed under the `assets` directory e.g. `assets/css/first.css`.

```toml
[params]
	customcss = ["css/first.css", "css/second.css"]
```


## Config of the Demo Site

```toml
baseURL = "https://duarte2025.github.io/Teko/"
languageCode = "en-us"
title = "Teko"
theme="Teko"
copyright = "© William M Duarte"
# Code Highlight
pygmentsstyle = "monokai"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true

disqusShortname = "yourDisqusShortname"

paginate=3 # articles per page

[params]
	mode="auto" # color-mode → light,dark,toggle or auto
	useCDN=false # don't use CDNs for fonts and icons, instead serve them locally.
	subtitle = "Minimal and Clean [blog theme for Hugo](https://github.com/duarte2025/teko)"
	mathjax = true # enable MathJax support
	katex = true # enable KaTeX support

# Social Tags

[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/duarte2025/teko"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://twitter.com/duarte2025/"

[[params.social]]
name = "GitLab"
icon = "gitlab"
url = "https://gitlab.com/duarte2025/"

# Main menu Items

[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4
```
---

