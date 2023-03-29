---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Clock_1
title: E-Paper-Clock

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":Cricket2_Front_View.jpg"
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

This project is intended to be a low power clock,
Suitable to use as a travel clock, and also suitable as a room clock.
An internet Access Point is needed for proper operation. 
To acheive this an E-Paper display is used, along with an RPi2040 processor.
The processor only updates the display once per minute, and
and otherwise is idle and the processor hibernates.

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


TLV62569 3.3V Buck Converter Breakout - 3.3V Output 1.2A Max (ADA4711)

This little buck converter based on the TLV62569 3.3V is super handy, taking up to 5.5V input and providing a 3.3V output with up to 1.2A continuous current.
£11.70
Raspberry Pi Official USB-C Power Supply - UK – White (RPI-069)


RV3028 Real-Time Clock (RTC) Breakout (PIM449)

An ultra-low-power ( ~100 nA), highly accurate real-time clock breakout. The RV3028 RTC breakout is perfect for adding timekeeping to your project and, thanks to the tiny on-board battery, it'll keep time when your device is powered off. Like all the best timepieces, it's Swiss-made!


### Lists

- The LiFePO4 battery is used as it makes implementation easier
And makes the 3 months battery life easier to achieve 
- The MQTT message system outputs a single JSON message, 
this is to make better use of battery life, and makes post p
- 

***

![E-Paper-Clock_Prototype](:E-Paper-Clock_Prototype.jpg){:data-align="center"}

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
