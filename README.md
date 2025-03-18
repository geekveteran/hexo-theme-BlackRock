# hexo-theme-BlackRock
A simple hexo theme

## Install

### Install Theme 

```shell
$ git clone https://github.com/geekveteran/hexo-theme-BlackRock.git
themes/BlackRock
```

### UseTheme

Hexo（`hexo/_config.yml`）change the theme setup in `themes/BlackRock`。
```  bash
theme: BlackRock
```

###  Update

``` bash
cd themes/BlackRock
git pull
```

### About Page

``` shell
$ hexo new page 'about'
```

# About page
about:
  photo_url: '/themeauthor.jpg' ## Your photo e.g. /themeauthor.jpg
  items:
  - label: email
    url: 'mailto:chaoles@foxmail.com'  ## Your email with mailto: e.g.  mailto:chaoles@foxmail.com
    title: 'chaoles@foxmail.com' ## Your email e.g.  chaoles@foxmail.com
  - label: github
    url: 'https://github.com/geekveteran' ## Your github'url e.g.  https://github.com/geekveteran
    title: 'geekveteran' ## Your github'name e.g.  geekveteran

### localSearch
Install[hexo-generator-json-content](https://github.com/alexbruno/hexo-generator-json-content)Creat JSON Search File，and add the config into `hexo/_config.yml`：
```shell
$ npm install hexo-generator-json-content --save
```
and then `hexo/_config.yml`add config：
```YAML
jsonContent:
  meta: false
  pages: false
  posts:
    title: true
    date: true
    path: true
    text: true
    raw: false
    content: false
    slug: false
    updated: false
    comments: false
    link: false
    permalink: false
    excerpt: false
    categories: false
    tags: true
```

## License
[MIT License](LICENSE)