---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_E_Cigarette_Battery_Eliminator
title: E-Cigarette Battery Eliminator

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":torch_in_bits1.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-10-30 08:11:06 +0900

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

This is a simple idea to re-use the batteries from a disposable E cigarette and make a cheap and useful
battery eliminator. The circuit uses a cheap chinese module that provides battery protection, a micro USB to charge 
the battery, and a boost circuit, so the unit can replace 6v to 12v batteries.

As the circuit/battery is permanently in circuit, an on/off switch is required, to maintain the battery power.

Two example installations are shown, for a Brother label printer, and a cheap Chinese multimeter.

<!-- outline-end -->

#### Brother Printer Installation

The case of the  torch(es) are well made, and have ample space for upgrading / rework.

**Keep it simple**, replace the small incandescent bulb with an LED, 
this will be driven directly by XXX Lithium batteries, try to keep the mounting of these batteries simple.
A protection / driver module will be required.
Keep the single button for ON/OFF operation.
Add a recharge connector in the handle.

![Complete Battery Eliminator](:BrotherPrinter1.jpg){:data-align="center"}

![Battery Eliminator Detail](:BrotherPrinter2.jpg){:data-align="center"}

![Exposed Battery Eliminator](:BrotherPrinter3.jpg){:data-align="center"}

#### Multimeter Installation

![Meter Battery Eliminator Fitting](:Meter1.jpg){:data-align="center"}

![Complete Meter Battery Eliminator Fitting](:Meter2.jpg){:data-align="center"}

### Applicable Links

Link to project page [Torch Rework](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme).
