---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Hallway_Light
title: Hallway Light

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":Hallway_Light_Open.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-03-29 08:11:06 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-02-10 08:11:06 +0900
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

The Hallway Light incorporates LEDs and a Loudspeaker
The unit can function as a doorbell, and as a nightlight.



<!-- outline-end -->

### PCBs

![Cricket2-Main-PCB-Front](:E-Paper-Clock_PCB_Front.jpg){:data-align="center"}

![Cricket2-Main-PCB-Back](:E-Paper-Clock_PCB_Back.jpg){:data-align="center"}

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

***

### Paragraphs


### Lists

- The LiPo battery is a salvaged unit from an e-cigarette.



- 1


***

![E-Paper-Clock_Prototype](:E-Paper-Clock_Prototype.jpg){:data-align="center"}

### USB connectors

Three USB connectors are present.

- 1 The RP2040 USB connector can power the unit, it's also used to program the RP2040.
- 2 The TP4056 board USB is for charging the LiPo battery.
- 3 The externally available USB is for day to day running of the clock from an external power source.
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
