---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_433MHzTester
title: Telegram Reporter Sentry

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":uk_map.png"
# disable comments on this page
#comments_disable: true

# publish date
date: 2025-09-22 07:11:06 +0900


# seo
# if not specified, date will be used.
#meta_modify_date: 2025-09-22 07:00:06 +0900
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

# Outline


This project was designed to fulfill two main functions, to emulate a number keypads and discreet 433MHz buttons, 
and to intercept these codes when transmitted, so it acts as both a transmitter and receiver.

It can function as a development tool, and as a replacement for existing keypads and other hardware.

The project was designed to reuse elements of the Telegram Reporter project as far as is practical,
this included the schematic and PCB design, and also the software.

The project fits in the same calculator housing as the Telegram reporter, this is an AliExpress calculator kit, 
which provides the housing, display the buttons.

# Images

![Unit pPrior to assembly](:433MHzTesterBuild1.jpg)

# PCB

# Build Notes

Aero Pins are used to connect the power from the USB connector to the keypad board, these are cut back,
because clearance is very limited between the 1602A display and the keypad board.
Also the DIL pins on the 1602A display need to be trimmed back or the unit will not close.

# Operation Notes

Fourmodes of operation are provided, selected by keys A-D after power up.

# Applicable Links

--
Sent with GMX Mail app


