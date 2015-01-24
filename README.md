## Clean blog theme - Spress version

Clean blog theme is a ported theme to Spress design by [Start Bootstrap](http://startbootstrap.com/).

[Live demo](http://spress-add-ons.github.io/clean-blog/).

### Features

* Fully responsive
* Distraction free blog text optimized for legibility.
* Working with [getsimpleform](https://getsimpleform.com/) contact form with validation.
* Comments powered by [Disqus](disqus.com).

### How to install?

#### Download a copy

* Get a copy of the latest [release](https://github.com/spress-add-ons/Clean-blog-theme/releases).
* Uncompress it.
* Go to `Clean-blog-theme` folder
* `spress site:build --server --watch`

#### With Git

* [Fork this repository](https://github.com/spress-add-ons/Clean-blog-theme/fork)
* Clone it: ` https://github.com/YOUR-USER/Clean-blog-theme.git
* Go to `Clean-blog-theme` folder
* `spress site:build --server --watch`

#### Globally

**This options is not available with `spress.phar`**.

Go to your [Spress](http://spress.yosymfony.com/) installation folder i.e  **~/Spress** and add the following depencency to your `composer.json` file 

```json
"require": {
    "spress-add-ons/Clean-blog-theme": "1.0.*@dev"
}
```

and then run the following command to install the dependency.

```bash
$ composer update
```

Next create your new site:

```bash
$ spress new:site /your-site-dir clean_blog
$ cd /your-site-dir
$ spress site:build --server --watch
```

## Configuration

### Comments

Comments are powered by [Disqus](disqus.com) and it need your 
**disqus shortname**. To get it, you need create a account at this service.
It's free.

```yaml
comments:
  enabled: true
  disqus_shortname: yosymfony
```

### Top menu

Top menu are composed by each of **pages with `title` attribute**. e.g: `about/index.html`:

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

To create a new post use `new:post` command from Spress:

```bash
$> spress new:site
```

Each post has a header image. You can configure your image and some data about it.

```yaml
header_img:
  url: "img/post-bg-07.jpg"
  author: Yuri Samoilov
  author_url: https://flic.kr/p/mjhDwB
```

## License

[Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0).
