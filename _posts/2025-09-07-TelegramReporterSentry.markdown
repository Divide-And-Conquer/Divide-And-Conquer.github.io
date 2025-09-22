---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_TelegramReporterSentry
title: Telegram Reporter Sentry

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
date: 2025-09-21 07:11:06 +0900


# seo
# if not specified, date will be used.
#meta_modify_date: 2025-09-21 07:00:06 +0900
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


Todo: show  complete unit.

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


This unit is to provide a texting style capability to somebody that struggles when using/understanding a mobile phone, and cannot text for themselves.

It allows the user to send a number of predefined messages that are sent to the mobile messaging platform called telegram. Telegram will provide notification that a message has been received.

In addition allows an emergency message to be broadcast from a "panic" button, or send a message on a specific event like a doorbell press. or smoke detector.

Typical messages might be, I've gone to sleep, l need milk,I need a newspaper, something in the house doesn't work.

The receiver of the message can then ring the user if necessary and clarify the situation.

This project shares the same pcb as 433MHz tester.

ChatGPT used extensively during the software design, and some aspects of the hardware design.

The Arduino framework is used for this project.

ChatGPT was especially useful for the asynchronous operation of the project.Wi-Fi, sending and receiving is  handled on CPU 0. Decoding the 443MHz signals and keypad handling is on cpu 1.

An asynchronous posting mechanism is used to send the Telegram messages.So messages are not lost.
This currently has a depth of five messages.

In principle the receiver of the messages can send messages to the unit, the underlying code for this is present.

Telegram messages can be tagged as Informational, Alert, or Critical Alert which is intended for panic buttons, smoke detection, and similar events.
