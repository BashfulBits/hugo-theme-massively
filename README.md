# Hugo Theme Massively MBR

My fork of [Curtis Timson's Massively theme] for use with the [Hugo static site generator](https://gohugo.io/).

![Hugo Theme Massively screenshot on Desktop, Tablet and Mobile](images/device-screenshots.png)

## Demo

I'm using my fork of the theme on my personal site at https://marcelbrueckner.de/

## Setup

### Configuration

See my personal site configuration as an example:

[https://gitlab.com/marcelbrueckner/marcelbrueckner.gitlab.io](https://gitlab.com/marcelbrueckner/marcelbrueckner.gitlab.io)

#### Hugo Internal Templates

The theme currently also supports the following ["internal templates" supplied by Hugo](https://gohugo.io/templates/internal/)

- [Disqus](https://gohugo.io/templates/internal/#disqus)
- [Google Analytics](https://gohugo.io/templates/internal/#configure-google-analytics)

### Cover Image

The cover image will be resized for different screen sizes and thus needs to be retrieved as a resource. For this, Hugo requires to load the file from the `assetDir` (which is `/assets` by default). The background image is expected to be stored in an subfolder called `images/`, so have to add an image to the following location in your Hugo application:

```plain
/assets/images/YOUR_BACKGROUND_IMAGE.EXT
```

In your site's parameters, provide the image name via `backgroundImage = YOUR_BACKGROUND_IMAGE.EXT`.

### Supported Languages

- [English](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/en.toml)
- [French](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/fr.toml)
- [German](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/de.toml)
- [Japanese](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/ja.toml)
- [Simplified Chinese](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/zh.toml)
- [Spanish](https://github.com/curttimson/hugo-theme-massively/blob/master/i18n/es.toml)

## Custom Front Matter

- `disableComments` - If set to `true` this will disable comments on the post when Disqus is enabled.

## Changes to the original hugo-theme-massively

- [@6a6e965](https://github.com/marcelbrueckner/hugo-theme-massively/commit/6a6e965d547630bb35fbb758dcb6dc21a57eeb40) Disable parallax scrolling effect by default as the background image was constantly bouncing around
- [@627f245](https://github.com/marcelbrueckner/hugo-theme-massively/commit/627f245faa45e47702678705ada327cc24872af4) Make copyright messages customizable in order to
  - use custom copyright text (instead of site title)
  - give attribution to cover photo author
- [@fbc4b74](https://github.com/marcelbrueckner/hugo-theme-massively/commit/fbc4b748011d74794c5d78d4c77c6169e23f68ed) Make background image path customizable (thanks to [Jonathan Keane](https://github.com/jonkeane) from which I borrowed ~~some~~ [a lot of code](https://github.com/jonkeane/hugo-theme-massively-jtk/blob/7478c65b03ec912ebdb44c61b5abc55badfbb5ff/layouts/partials/bg.html))
- [@82ed505](https://github.com/marcelbrueckner/hugo-theme-massively/commit/82ed50553a781e106005c40480cc49ce5d85a588), [@99c1407](https://github.com/marcelbrueckner/hugo-theme-massively/commit/99c14077f16de86f21a14854d64afde25c6d6ad2) Update Font Awesome from v4.7.0 to v5.12.0
- [@5ee863a](https://github.com/marcelbrueckner/hugo-theme-massively/commit/5ee863abdec563dbbf5bcedd87bf0a2869c94df9) Enable use of a list of arbitrary links to social profiles instead of a predefined set
- [@b5def44](https://github.com/marcelbrueckner/hugo-theme-massively/commit/b5def443901d73d3169d4452553e42880feeb902), [@6e0703d](https://github.com/marcelbrueckner/hugo-theme-massively/commit/6e0703d5a238ca4795e3c47098ebe1637601df75), [@77debfd](https://github.com/marcelbrueckner/hugo-theme-massively/commit/77debfd8c451a56c80c3e919cd096068b36d4184) Rewrite layout using Hugo's [Base Templates](https://gohugo.io/templates/base/), add support for sections and additional links in navigation
- [@4c7d5d8](https://github.com/marcelbrueckner/hugo-theme-massively/commit/4c7d5d83e9daea34d6da274564c49f2f00070116) Add Git info support
- [@ccd1d87](https://github.com/marcelbrueckner/hugo-theme-massively/commit/ccd1d878d4ca1e3d58bb4bb92ba70f9b8e4989b0) Add German language support

## Credits

- [Massively by HTML5 UP](https://html5up.net/massively)
- Curtis Timson for his fundamental work on [hugo-theme-massively](https://github.com/curtistimson/hugo-theme-massively)
- [Jonathan Keane](https://github.com/jonkeane) for some inspiration I've got from his [very own fork](https://github.com/jonkeane/hugo-theme-massively-jtk) of the Hugo Theme Massively

## License

This hugo theme is licensed under the [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).

Read More - [LICENSE](LICENSE)
