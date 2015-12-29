---
layout: post
title: "Welcome to Spress"
subtitle:   "Spress is the static site generator in PHP"
date:       "2015-01-23 21:00:00"
author:     "Spress add-ons"
header_img:
  url: "assets/img/post-bg-07.jpg"
  author: Yuri Samoilov
  author_url: https://flic.kr/p/mjhDwB
---
To create a new post, simply runs `spress new:post` command or adds a file
in the `./src/content/posts` folder that follows the convention `YYYY-MM-DD-name-of-post.md`.

## Comments

Comments are powered by [Disqus](disqus.com) and they need a 
**disqus shortname**. To get it, you need to create an account at this service and
next edit the `config.yml` filename:

```yaml
comments:
  enabled: true
  disqus_shortname: "your-shortname"
```

## About Spress:

* [Spress](http://spress.yosymfony.com)
* [Github](http://github.com/spress)

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/spress/Spress?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)