---
layout: post
title: "I'm a developer"
subtitle:   "Syntax highlighting using Javascript"
date:       "2015-01-23 20:00:00"
author:     "Spress add-ons"
header_img:
  url: "assets/img/post-bg-07.jpg"
  author: Yuri Samoilov
  author_url: https://flic.kr/p/mjhDwB
tags:
  - spress
categories:
  - news
---
Are you a developer? so you are lucky because Simple theme come with syntax highlighting powered
by [Highlight js](https://highlightjs.org) with support for over 100 languages. See a example
code in PHP:

```
use Yosymfony\Spress\Core\Spress;

class MyClass
{
    public function parseSite()
    {
        $spress = new Spress();
        $spress['spress.config.site_dir'] = '/path-to-your-spress-site';
        $spress->parse();
    }
}
```
