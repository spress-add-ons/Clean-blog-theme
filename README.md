## Clean blog theme - Spress version

Clean blog theme is a ported theme to Spress designed by [Start Bootstrap](http://startbootstrap.com/).

[Live demo](http://spress-add-ons.github.io/clean-blog/).

This theme requires Spress >= 2.0.

### Features

* Fully responsive.
* Distraction free blog text optimized for legibility.
* Contact form powered by [getsimpleform](https://getsimpleform.com/).
* Comments powered by [Disqus](disqus.com).

### How to install?

#### Download a copy

* Get a copy of the latest [release](https://github.com/spress-add-ons/Clean-blog-theme/releases).
* Uncompress it.
* Go to `Clean-blog-theme` folder
* `spress site:build --server --watch`

#### Git

* [Fork this repository](https://github.com/spress-add-ons/Clean-blog-theme/fork)
* Clone it: ` https://github.com/YOUR-USER/Clean-blog-theme.git
* Go to `Clean-blog-theme` folder
* `spress site:build --server --watch`

## Configuration

### Comments

Comments are powered by [Disqus](disqus.com) and they need a 
**disqus shortname**. To get it, you need to create an account at this service.
It's free.

```yaml
comments:
  enabled: true
  disqus_shortname: your-shortname
```

### Top menu

The top menu is composed by each of **pages with `title` attribute**. e.g: `about/index.html`:

```yaml
title: "About me"
```

### Contact form

The contact form is a AJAX form configured in `config.yml`:

```yaml
forms:
    contact:
        getsimpleform_api_token:
```

You need a API key from [getsimpleform](https://getsimpleform.com/) service. It's free.

### Writing a post

To create a new post, runs `new:post` command from Spress:

```bash
$> spress new:site
```

Each post has a header image. You can configure your image and some data about it.

```yaml
header_img:
  url: "assets/img/post-bg-07.jpg"
  author: Yuri Samoilov
  author_url: https://flic.kr/p/mjhDwB
```

## License

[Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0).
