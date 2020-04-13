# Light Speed

An insanely fast and performance-based Zola theme, ported from [Light Speed Jekyll](https://github.com/bradleytaunt/lightspeed).

Some fun facts about the theme:

* Perfect score on Google's Lighthouse audit
* Only ~434 bytes of CSS
* No media queries
* No JavaScript

Demo: [quirky-perlman-34d0da.netlify.com](https://quirky-perlman-34d0da.netlify.com)

-----

## Contents

- [Installation](#installation)
- [Options](#options)
  - [Title](#title)
  - [Sass](#Sass)
  - [RSS](#RSS)
  - [Footer menu](#footer-menu)
- [Original](#original)
- [License](#license)

## Installation
First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/carpetscheme/lightspeed.git
```
and then enable it in your `config.toml`:

```toml
theme = "lightspeed"
```

Posts should be placed in the `blog` folder.

## Options

### Title
Set a tile and description for your site to appear in the header:

```toml
title = "Different strokes"
description = "for different folks"

```

### Sass

The theme's css is compiled from sass and the output is imported inline to the header :zap:

You can overide the styles by enabling sass compilation in the config:

```toml
compile_sass = true
```

...and placing a replacement `style.scss` file in the sass folder.

### RSS
Enable rss with the standard zola option:

```toml
generate_rss = true
```

...and include your name and email in the feed by setting fields in `extra` with keys `author` and `email`:

```toml
[extra]

author = "Grant Green"
email = "grant@green.org"
```

### Footer-menu
Set a field in `extra` with a key of `footer_links`:

```toml
[extra]

footer_links = [
    {url = "$BASE_URL/about", name = "About"},
    {url = "$BASE_URL/rss.xml", name = "RSS"},
    {url = "https://google.com", name = "Google"},
]
```

If you put `$BASE_URL` in a url, it will automatically be replaced by the actual
site URL.

## Original
This template is based on the Jekyll template [Light Speed Jekyll](https://github.com/bradleytaunt/lightspeed) by **Bradley Taunt**:

- <https://github.com/bradleytaunt>
- <https://twitter.com/bradtaunt>


## License

Open sourced under the [MIT license](LICENSE.md).

This project is open source except for example articles found in `content`.

