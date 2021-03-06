# hexo-theme-overdose
[![GitHub release](https://img.shields.io/github/release/hyunseob/hexo-theme-overdose.svg?maxAge=2592000?style=plastic)](https://github.com/HyunSeob/hexo-theme-overdose)
[![license](https://img.shields.io/github/license/hyunseob/hexo-theme-overdose.svg?maxAge=2592000?style=plastic)](https://github.com/HyunSeob/hexo-theme-overdose)

[Demo](http://hyunseob.github.io)

⚠ Caution: you could be overdosed with this hexo theme.

![Mock-up image](/source/images/mock-up.png)

The Overdose is minimalistic, simple and beatiful hexo theme, specialized in Korean blogs.

This theme works with hexo v3.2 or later and Node v7 or lower.

## Features

- Responsive design
- Lightweight, not using jQuery or underscore.js, etc.
- Various code highlighting theme (Thanks to @SungYeolWoo), Set [Dracula](https://draculatheme.com/) theme by default
- [Font setting](#font-setting)
  - noto-sans-kr
  - spoqa-han-sans-kr
  - spoqa-han-sans-jp
- SEO friendly
  - canonical link
  - [Schema.org](https://schema.org) markup
- With other services
  - Google Analytics
  - Google Site Verification
  - Naver Site Verification
  - [Disqus](#disqus)
- Related posts
- Dynamic hide/show menu (Unstable)
- Sharing(Facebook, Twitter, Pinterest, Pocket)

## Quick Start

### Installation
First, clone this repository.
```
$ cd your/hexo/directory
$ git clone https://github.com/HyunSeob/hexo-theme-overdose.git themes/overdose
```

The overdose theme is using jade/sass(with bourbon). So install renderers.
```
$ npm install --save hexo-renderer-jade hexo-renderer-bourbon
```

And initialize this theme.
```
$ cd themes/overdose;node init
```

And then, specify `overdose` theme in your root configuration file.

``` yml
theme: overdose
```

Finally, start the hexo server and enjoy.
```
$ hexo server
```

### Font setting
You could choose from the following options.  
After install, you should set font config in themes/overdose/_config.yml
```yaml
# Font
## availableFontList: [
##   'noto-sans-kr',
##   'spoqa-han-sans-kr',
##   'spoqa-han-sans-jp'
## ]
## If you don't want font, you shouldn't specify the font.
font:
```
* noto-sans-kr
```bash
npm run noto-kr
```
* spoqa-han-sans-kr
```bash
npm run spo-kr
```
* spoqa-han-sans-jp
```bash
npm run spo-jp
```
* Korean fonts(noto-sans-kr, spoqa-han-sans-kr)
```bash
npm run font-kr
```
* Spoqa fonts(spoqa-han-sans-kr, spoqa-han-sans-jp)
```bash
npm run spoqa
```
* All fonts(noto-sans-kr, spoqa-han-sans-kr, spoqa-han-sans-jp)
```bash
npm run font
```

### Configuration

See the [_config.yml.example](https://github.com/HyunSeob/hexo-theme-overdose/blob/master/_config.yml.example) file.

## Disqus

``` yml
# _config.yml of base, not theme config
# Please put your shortname of disqus here.
disqus_shortname:
```

### Post Front matter

You can set the post banner image by `banner` property.

``` yml
---
title: Overdose is a hexo theme
date: 2016-09-10 14:30:00
banner:
  url: /images/default.jpg
  width: 1280
  height: 720
categories:
  - Blog
  - Hexo
tags:
  - Hexo
---
```

## Browser compatibility

- [x] Chrome
- [x] Edge
- [x] IE 9+ (CSS3 Animation is not worked in IE9)
- [x] Firefox
- [x] Safari
- [x] Android Browser
- [x] iOS Safari

## To Do

- i18n
- LiveRe
- Facebook Comments
- Featured posts
