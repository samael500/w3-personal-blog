Personal Blog a Blogging Category Flat Bootstrap Responsive Web Template
---

Pelican adaptation of W3 Personal Blog template. [Live demo](http://samael500.github.io/).

![index](readme_img/index.png)
<hr />
![article](readme_img/article.png)
<hr />
![archive](readme_img/archive.png)


[Personal Blog](https://w3layouts.com/personal-blog-a-blogging-category-flat-bootstrap-responsive-web-template/)
is a clean, flat and professional Blogging category template for
bloggers and blogging website. It can be customized easily to suit your wishes.
It comes with a free Flat Responsive web design template.
You can use this template for any type of websites.

Personal Blog web template is built in a Fancy style however it can be used
as per the user requirements. Personal Blog designed with a clean flat grid
system. It is compatible in all web browsers,Smartphones and Tablets.It is
designed using HTML5 and CSS3.

###Template Information
- **Template Name:** Personal Blog a Blogging Category Flat Bootstrap Responsive Web Template
- **Licence:** Life Time Free Licence under Creative Commons Attribution 3.0
- Unported. Unlimited Use, Source files & PSD included, you can help & support us
- (W3Layouts, a Non-Profit) by donations or you should keep link to our website.
- **Date Created:** Feb 21, 2015
- **Compatible Browsers:** Google Chrome, Firefox, Safari, IE, Opera etc
- **High Resolution:** Yes
- **Layout:** Fluid Responsive Layout
- **Source Files included:**  HTML files (.html), Style Sheets (.css), Images (.jpg/png/gif),
- **Tags:** Free Responsive Template, free responsive templates download, free
responsive mobile templates, free html5 css3 templates, free fluid responsive
themes, single flat Responsive web template, cross-browser compatible web
template, best responsive template.
- **Download PSD:** [Here](http://www.alltemplateneeds.com/psd-templates/free-psd-website-template/free-psd-110.html)

This entry was posted in [Blogging Template](https://w3layouts.com/blogging-template/).

###Article image
On the main page of the article is displayed with a preview image. To specify the image to add to the meta tag information `Image`.

![article_info](readme_img/article_info.png)

For example:
```Markdown
Title: Ралли на браузерах
Date: 2015-04-01 10:20
Modified: 2015-04-05 19:30
Category: Python
Tags: python, browsers, wb-tech
Image: /media/browsers/pedestal.png
Summary:
    Собственный проект [WB--Tech](http://wbtech.pro/) по комментированию
    скриншотов [coment.me](http://coment.me/) на сегодняшний день, для получения
    снимка сайта использует связку `selenium + firefox`. Данный подход решает
    задачи получения скриншота, однако тратит достаточно много памяти, и к тому же
    со временем накапливается большое количество повисших процессов, что в свою
    очередь приводит к подвисанию сервиса. В связи с этим, необходимо исследовать
    доступные варианты и определить наилучший из браузеров для автоматического
    создания скриншотов...
#

```

###Pelican conf
It is my pelicanconf.py file:
```python
#!/usr/bin/env python
# -*- coding: utf-8 -*- #
from __future__ import unicode_literals

AUTHOR = u'Maks'
SITENAME = u'Maks blog'
# SITESUBTITLE = u'Samael500'
SITEURL = 'http://samael500.github.io'
KEYWORDS = u'Samael500 personal blog'

PATH = 'content'

TIMEZONE = 'Europe/Moscow'

DEFAULT_LANG = u'ru'

# Feed generation is usually not desired when developing
FEED_DOMAIN = SITEURL

# Blogroll
LINKS = (
    ('Pelican', 'http://getpelican.com/'),
    ('Python.org', 'http://python.org/'),
    ('Jinja2', 'http://jinja.pocoo.org/'),
    # ('You can modify those links in your config file', '#'),
)

# Social widget
SOCIAL = (
    ('<i class="fa-li fa fa-vk"></i> ВКонтакте', 'https://vk.com/id44829586'),
    ('<i class="fa-li fa fa-facebook"></i> Facebook', 'https://www.facebook.com/100009559792869'),
    ('<i class="fa-li fa fa-twitter"></i> Twitter', 'https://twitter.com/samael500'),
    ('<i class="fa-li fa fa-github"></i> Github', 'https://github.com/samael500'),
)

# TWITTER_USERNAME = 'samael500'

DEFAULT_PAGINATION = 10

# Uncomment following line if you want document-relative URLs when developing
RELATIVE_URLS = True

THEME = '../w3-personal-blog'
GITHUB_URL = 'https://github.com/Samael500'

STATIC_PATHS = ['icons', 'media', 'extra', 'emojify', 'stuff', ]

TYPOGRIFY = True

DISPLAY_PAGES_ON_MENU = True

GOOGLE_CUSTOM_SEARCH = '006263355362628034990:cuxoisonrno'


ARTICLE_URL = u'articles/{category}/{slug}/'
ARTICLE_SAVE_AS = u'articles/{category}/{slug}/index.html'

PAGE_URL = u'{slug}/'
PAGE_SAVE_AS = u'{slug}/index.html'

AUTHOR_URL = u'author/{slug}/'
AUTHOR_SAVE_AS = u'author/{slug}/index.html'

AUTHORS_URL = u'authors/'
AUTHORS_SAVE_AS = u'authors/index.html'

CATEGORY_URL = u'category/{slug}.html'
CATEGORY_SAVE_AS = u'category/{slug}.html'

TAG_URL = u'tag/{slug}/'
TAG_SAVE_AS = u'tag/{slug}/index.html'


PLUGINS=['plugins.sitemap', ]

SITEMAP = {
    'format': 'xml',
    'priorities': {
        'articles': 0.5,
        'indexes': 0.5,
        'pages': 0.5
    },
    'changefreqs': {
        'articles': 'weekly',
        'indexes': 'daily',
        'pages': 'monthly'
    }
}
```