# Beautiful-hexo

Beautiful-hexo is a simple elegant hexo theme ported from [Beautiful-jekyll](http://deanattali.com/beautiful-jekyll) which written by [Dean Attali](http://deanattali.com/aboutme). Nice work!

![hexo-preview](images/hexo-preview.png)

### Install

```
hexo init site 
cd site
npm install --save hexo-generator-archive hexo-renderer-jade hexo-generator-tag hexo-generator-feed hexo-generator-sitemap hexo-browsersync 
git clone --depth 1 https://github.com/twoyao/beautiful-hexo.git themes/beautiful-hexo
```


Modify `_config.yml` change `theme` to `beautiful-hexo` and configure hexo-generator-archive :

```
theme: beautiful-hexo

archive_generator:
    per_page: 0
    yearly: false
    monthly: false
    daily: false
```

### Comment

#### netease-gentie

Setup `comment.netease.productKey` in theme's `_config.yml`. For test, you have to ensure your website hostname match settings of netease-gentie. 
To do so, add flollowing lines in /etc/hosts:

```
127.0.0.1 notes.example.com
```

And run hexo at 80 port: `sudo hexo s --debug -p 80`. After test, you may revert hosts file.

### Tags page

For displaying a page with all blog tags, create a folder named `tags` at `source` folder with the following `index.md` inside:


```
---
title: "Tags"
layout: "tags"
---
```

Don't forget to update your `navbar-links` at `beautiful-hexo` `_config.yml` file:

```
navbar-links:
    ...
    Tags: /tags
```

Theme config file is brief and clear. 
If you have any question, check [hexo online document](https://hexo.io/).

