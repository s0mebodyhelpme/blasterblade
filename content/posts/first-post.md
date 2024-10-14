---
title: "Introduction: How to Make a Hugo Website"
date: 2024-10-14T03:07:37+08:00
tags: [Hugo, Static Site]
featured_image: "/images/internet.jpg"
description: "A tutorial on making a website powered by Hugo."
---

### Intro of the Intro

With the growing accessibility of knowledge in making websites, it seems useful to make a tutorial on making one for Hugo, a very powerful and performant static website generator, which this site itself is powered by. So, without further delay, here's a tutorial on making a Hugo Website.

### What this Tutorial DOES NOT Intend to Cover

We won't be covering the administrivia of setting up a domain name and linking it up to your server. That deserves its own tutorial. Certbot, nginx, apache2, caddy, etc. will be saved for another day.

### What this Tutorial INTENDS TO COVER

We'll be going over the basics of installing hugo, setting up a basic template, and installing a theme.

#### Installation

You can "install Hugo on macOS, Linux, Windows, BSD, and on any machine that can run the Go compiler tool chain," as the Hugo [website](https://gohugo.io/installation/) states. Go visit that hyperlink to find the install instructions for your OS and come back here.

#### Initialization

You can initialize a hugo website with the following command, replacing yoursitenamehere with the name you wanna give to your site's folder and title (the latter of which you can change in the hugo.toml file):

``` 
hugo new site yoursitenamehere
```

#### Installing themes

Browse the themes at the hugo [website](https://themes.gohugo.io/) and pick one that speaks to you. The installation instructions and dependencies will differ, but generally speaking the way to install a hugo theme via git is the following:

```
git clone https://github.com/authorname/themename themes/themename
```

With the values for _authorname_ and _themename_ being subsituted for the author and name of the theme you wish to use.

#### You're ready

With that, you should have a good starting point in making a Hugo website. From there, configure your hugo.toml to reflect your domain name with the https:// prefix added to the beginning, set the **theme** value to your themename value, etc.

#### Tips

Always, always, ALWAYS read the DOCS! This is the best advice I can give you. Read the docs of both Hugo and your used theme to get a better understanding of how they work and how you can use them.


### Closing

That's all for now. God bless

{{< chat >}}
