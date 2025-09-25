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
tags: [pico-w, e-paper]
# thumbnail image for post
img: ":E-Paper-Clock_Front.jpg"
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

# Outline

This project is intended to be a low power clock,
suitable to use as a travel clock, and also suitable as a room clock.

This unit uses an E-Paper display, along with an RPi2040 processor,
and is powered by a LiPo battery. An on-board battery charger is present,
this charges the battery using a USB power source.

The processor only updates the display once per minute, and hibernates
between updates to maximise the battery life.

The unit updates it's time once a day from the internet.

A diagnostic mode / interface is also built-in, this allows
a pair of Wi-Fi access Point SSID/Passwords to be entered/stored.

To build this unit in the slim case (portable drive case), I had to cut the RP2040 connector off the back of the board.

Todo: show  complete unit in its case.

Todo: show  RP2040 connector off the back of the board.

<!-- outline-end -->


# Design Notes

- 1 The RP2040 USB connector can power the unit, it's also used to program the RP2040.
- 2 The TP4056 board USB is for charging the LiPo battery.
- 3 The externally available USB is for day to day running of the clock from an external power source.

The software libraries for the E-Paper display require the Raspberry Pi SDK and its associated development environment,
I had a lot of trouble getting on with this, and it curtailed my development of the item.

Special Font(s) had to be created for the display.

Todo: show Schematic

# Images

![Unit Prior to assembly](:E-Paper-Clock_Front.jpg)

### PCB

![E-Paper-Clock_PCB-Front](:E-Paper-Clock_PCB_Front.jpg){:data-align="center"}

![E-Paper-Clock_PCB-Back](:E-Paper-Clock_PCB_Back.jpg){:data-align="center"}

# Build Notes



# Operation Notes

# Development / Prototyping

This project was difficult to implement, primarily because of the RPi development framework being imature, and me
not wanting to learn it just for this one project. Also this was prior to RP introducing the debug probe, which would have helped.

![Development unit](:E-Paper-Clock_Prototype2.jpg)

It was also difficult mechanically to design an build, it took a lot of time.

![Development unit](:E-Paper-Clock_Prototype.jpg)

At least two itterations of PCBs were required.

# Applicable Links

[Waveshare 3.7inch E-Paper E-Ink Display Module for Raspberry Pi Pico, Black/White, 480×280 Pixels](https://www.youtube.com/watch?v=J_4rWR0zq_A)

https://www.waveshare.com/wiki/Pico-ePaper-3.7#C_codes
tten how I did this, but it was with the help of some third party open source tools.

## Fontedit

I spent a lot of time generating some large Text Font characters for the display, and a celcius symbol. I have forgot.


[Make a new larger font for Waveshare SPI](https://wavesharejfs.blogspot.com/2018/08/make-new-larger-font-for-waveshare-spi.html)

[A desktop app to import, edit and export fonts as byte arrays for use in embedded systems](https://github.com/ayoy/fontedit)
[1](https://kapusta.cc/2020/03/20/fontedit/)
[2](https://kapusta.cc/2019/02/10/font2bytes/)



Todo: show case kit sites
