## Clean blog theme

Clean blog theme is a ported theme to Spress designed by [Start Bootstrap](http://startbootstrap.com/).

[Live demo](http://spress-add-ons.github.io/clean-blog/).

![Spresso theme preview](/screenshot.png)

### Features

* Fully responsive.
* Distraction free blog text optimized for legibility.
* Support for tags and categories in posts.
* Contact form powered by [getsimpleform](https://getsimpleform.com/).
* Comments powered by [Disqus](https://disqus.com).
* Code highlighted thanks to [highlight.js](https://highlightjs.org/).

## Installation
You can create a [site based on Clean blog](#creating-a-new-site-based-on-this-theme-creating-site)
or install this one as a theme of a [pre-existing site](#install-as-a-theme-of-pre-existing-site-pre-existing).

**Requirements:**
* Spress >= 2.2.0

### Creating a new site based on this theme

Performs the following command and clean-blog theme will be
installed in `mysite` folder:

```bash
$ spress new:site mysite spress-add-ons/clean-blog-theme
```

### Install as a theme of a pre-existing site

Go to your site folder and performs the following command:

```bash
$ spress add:plugin spress-add-ons/clean-blog-theme
```

And add this line to the `config.yml` file of your site:

```yaml
themes:
    name: "spress-add-ons/clean-blog-theme"
```

### How to update?

You can get the latest version of Clean blog theme with just run the following command:

```bash
$ spress update:plugin
```

## Contents
### Layouts

Refers to files within the `./src/layouts` directory, that define the architecture
of the content.

* `default.html`: The base layout. The derived layouts inject their contents
into this file at the line that says `{{ page.content }}`.
* `page.html`: Layout for pages.
* `post.html`: Layout for posts. They are located at `./src/content/posts`.
* `collection.html`: Layout used by collection pages: `categories.html` and `tags.html`.

### Includes

Refers to snippets of code within the `./src/includes` directory. These ones can
be inserted in layouts and pages.

* `head.html`
* `footer.html`
* `nav.html`
* `paginator.html`

## Configuration

### Comments

Comments are powered by [Disqus](disqus.com) and they need a
**disqus shortname**. To get it, you need to create an account at this service.
It's free.

```yaml
comments:
  enabled: true
  disqus_shortname: "your-shortname"
```

### Top menu

The top menu is composed by each of **pages with `title` attribute**.
e.g: `./src/content/about.md`:

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
$ spress new:post
```

Each post could has a header and thumbnail image. You can configure your image and some data about it.

```yaml
header_img:
  url: "assets/img/post-bg-07.jpg"
  author: "Yuri Samoilov"
  author_url: "https://flic.kr/p/mjhDwB"
```

#### Thumbnail images

The `index.html` page can display a thumbnail image for each post. This kind
of images must be located at `./src/content/assets/img` folder and the image
may has the dimentions `100x100 px`.

At the `thumb_img` key of each post you set the name of the image file:

```yaml
thumb_img: spress.png
```

## License

[Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0).
