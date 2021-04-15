---
title: "Creating Websites with Hugo"
date: 2021-04-06T15:51:03+05:30
---

## Hugo
Hugo is an open-source static site generator.
It is very fast, flexible and user friendly, but the best thing is you have many [themes and templates](https://themes.gohugo.io/) that will allow you to host static content website in minutes.

To install hugo in Ubuntu:
```
sudo apt-get install hugo
```
For other OS, Hugo has this extensive [Installation Guide](https://gohugo.io/getting-started/installing/).

To create a new site:
```
hogo new site <site name>
cd <site name>
```

Clone your favourite theme in `themes/` folder:
```
git init
git submodule add <theme's git repo> /themes/<theme's name>
```

Add your theme entry to	`config.toml` file:
```
...
theme = <theme's name>
```

Configure your theme according to the theme's page
and Start Hugo Server:
```
hugo server -D
```

If everything is successful, Go to `http://localhost:1313/` in your browser.