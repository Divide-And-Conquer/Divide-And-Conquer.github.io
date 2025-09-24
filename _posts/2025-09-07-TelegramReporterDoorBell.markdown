---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_TelegramReporterDoorBell
title: Telegram Reporter DoorBell

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":under-construction-site.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2025-09-07 07:11:06 +0900


# seo
# if not specified, date will be used.
#meta_modify_date: 2025-09-04 07:00:06 +0900
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

# Telegram Reporter DoorBell

The simplest use case for this project is the doorbell to telegram messenger.
This would pick up the 433 MHz signal from the doorbell push button
and send a message via telegram to be picked up on a mobile phone.
This could be extended using MQTT to track doorbell presses, and make actions happen within node-red.
This use case would allow existing cricket 3 PCB designs and hardware to be used(reused).

This project is created with the help of chatGPT.

The doorbell unit is positioned close to the Wi-Fi 6 router, a POE supply with a buck converter supplies 12V to both units.

The doorbell  internally uses a 12V to 5V converter taken from a car cigar lighter socket USB converter sold for £1 in Poundland.
This converter is an afterthought, that is why it is glued to the underside of th PCB.

This unit also has a test button, that makes a doorbell press message to be sent to Telegram.


can be used to check that Telegram messages are being transmitted/received.

![During Assembly](:Doorbell1.jpg)



<!-- outline-end -->

# Design Notes


Todo: show Schematic

# Images

![Unit Prior to assembly](:433MHzTesterBuild1.jpg)

# PCB

The PCB has been produced using KiCAD 9.0

# Build Notes


# Operation Notes


# Applicable Links

Todo: show calculator kit sites
