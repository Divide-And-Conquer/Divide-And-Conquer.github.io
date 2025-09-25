---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Cricket2
title: Cricket 2 - IOT Device

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [esp32, mqtt, iot]
# thumbnail image for post
img: ":Cricket2_Front_View.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-03-28 08:11:06 +0900

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

The original Cricket was a commercial project product made by the Things on Edge company based in Cambridge.

This device monitored it's own battery, temperature, and had a few inputs for measuring other external 
parameters, this added to the flexibility, and allowed the device to be customised. 
It then transmitted this monitored information to a server computer using MQTT. 
The original device was simple to deploy, low cost, and had a good battery life.

The company produced two versions of the Cricket device but unfortunately went out of business.
The version one device of theirs was configured via the internet and became unmodifiedable so was impossible to use
for further development. Also some of these devices just stopped working!

The version 2 device could still be reconfigured via a mobile phone or similar device.

Both devices kept in use for a number of months while whilst I came up with the design for the Cricket 2 replacement board. 

This project re-uses a PCB designed for a previous project of mine called Scheduler.
The PCB quite suitable for this purpose, and has many extra inputs, and capabilities way beyond the design of the original Crickets. 


<!-- outline-end -->


![IMG_20210107_124917](:Cricket1_Original.jpg){:data-align="center"}

#### Original Cricket Module fitted in 115x90x55 case 
{:data-align="center"}



### Original Cricket

Shown below is the original Cricket IOT device produced by Things On Edge.

![original Cricket](:Cricket1.jpg){:data-align="center"}

This device was simple to use, and ran for months on good AA batteries.
The Things On Edge company went bust, and operating these devices without their 
support became impractical.

### Cricket2 PCBs

This PCB was originally designed as a general purpose controller, as the boards were
not being used they provided an ideal platform to perform the Cricket2 role.

![Cricket2-Main-PCB-Front](:ESP32-Cricket2-Main-Board-Front.jpg){:data-align="center"}

#### Front View of PCB
{:data-align="center"}

![Cricket2-Main-PCB-Back](:ESP32-Cricket2-Main-Board-Back.jpg){:data-align="center"}

#### Rear View of PCB
{:data-align="center"}


### Design in more detail

The designed of Scheduler PCB  gave much greater headroom for expansion over the original Things on Edge product.

The ESP32 processor module handles the control of the device. The hibernation mode of the ESP32 is used to conserve battery power.
The hibernation is however quirky on the ESP32, and forces a program restart, and screws up any Wi-Fi connection established.

Because a program reboot is used, preserving parameters such as time is difficult, that is why an RV3028 RTC module is used,
this also has a little non volatile memory.

The RV3028 RTC module is ultra-low-power ( ~100 nA), and highly accurate.

real-time clock breakout. 
The RV3028 RTC breakout is perfect for adding timekeeping to your project and, thanks to the tiny on-board battery, 
it'll keep time when your device is powered off. Like all the best timepieces, it's Swiss-made!



Some changes / additions have been made with this implementation

### Lists

- The LiFePO4 battery is used as it makes implementation easier
And makes the 3 months battery life easier to achieve 
- The MQTT message system outputs a single JSON message, 
this is to make better use of battery life, and makes post p
- Orange


***

### Link



