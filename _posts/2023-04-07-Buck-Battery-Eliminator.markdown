---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Buck_Battery_Eliminator
title: Buck Battery Eliminator

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [LiPO_battery, buck_converter, development]
# thumbnail image for post
img: ":Buck-Battery-Eliminator-TLV62569.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-04-09 08:11:06 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2023-04-07 08:11:06 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
published: true
---

<!-- outline-start -->

The Buck converter is intended to provide a 3.3V power source, 
suitable for use as an AAA/AA battery eliminator, or general power source for electronics.
The TLV62569 buck converter IC provides a small and efficient device suitable 
to fit in the footprint of two AA batteries when paired with
a small Lithium cell.

<!-- outline-end -->



### Buck-Battery 

![Buck-Battery](:Buck-Battery-Eliminator-TLV62569.jpg){:data-align="center"}

#### TLV62569 module from Adafruit 
{:data-align="center"}








### Link

This is [Mr. Green Jekyll Theme](https://www.adafruit.com/product/4711), TLV62569 3.3V Buck Converter Breakout - 3.3V Output 1.2A Max.

\* Hello world! This is **[{{ site.data.owner[site.data.conf.main.default_lng].brand }}]({{ site.url }})**


#### Heading 4

##### Heading 5

###### Heading 6

***

### Paragraphs

### Lists

- Apple
- Banana
- Orange

1. Fruits
   1. Apples
      - Granny Smith
      - Mutsu
   1. Bananas
      - Cavendish
      - Red
1. Vegetables

***

### Tables

#### Small Table (centered)

| Fruits(not aligned) | Alignment (centered) | num (right align) |
| ------------------- | :------------------: | ----------------: |
| Apple               |       centered       |              9999 |
| Banana              |  centered long text  |               999 |
| Orange              |       centered       |                99 |
| Lemon               |       centered       |                 9 |
{:data-align="center"}

#### Wide Table (centered)

scroll enabled when page is narrow

| Fruits | num (left align) | num (right align) | num  | num  | num  |
| ------ | :--------------- | ----------------: | ---- | ---- | ---- |
| Apple  | 1111             |              1111 | 2222 | 3333 | 4444 |
| Banana | 111              |               111 | 222  | 333  | 444  |
| Orange | 11               |                11 | 22   | 33   | 44   |
| Lemon  | 1                |                 1 | 2    | 3    | 4    |
{:data-align="center"}

#### Wider Table

scroll enabled when page is narrow

| Fruits | num (left align) | num (right align) | num  | num  | num  | num  | num  | num  |
| ------ | :--------------- | ----------------: | ---- | ---- | ---- | ---- | ---- | ---- |
| Apple  | 1111             |              1111 | 2222 | 3333 | 4444 | 5555 | 6666 | 7777 |
| Banana | 111              |               111 | 222  | 333  | 444  | 555  | 666  | 777  |
| Orange | 11               |                11 | 22   | 33   | 44   | 55   | 66   | 77   |
| Lemon  | 1                |                 1 | 2    | 3    | 4    | 5    | 6    | 7    |

### Code

#### Highlight

{% highlight python %}
for i in range(5, 10):
  print(i)
{% endhighlight %}

#### Quote

```python
for i in range(5, 10):
  print(i)
```

