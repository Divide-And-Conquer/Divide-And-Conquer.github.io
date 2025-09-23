---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_SecurityCamera
title: Security Camera

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":YaleCameraHousing.jpg"
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

This project uses the case and various components from a ALL-IN-ONE_AW_01 Yale camera.

One serious difficulty when building your own camera is finding a suitable housing, especially one that can be mounted externally. Especially if the housing has to contain any extras (microphone/speaker/siren/PIR/second camera), the Yale camera unit has provision for these.

Sourcing a housing is difficult but you may be able to obtain one on eBay.

What components from the Yale unit can be reused?
- housing and mounting bracket
- PSU
- camera 
- IR LEDs
- siren
- speaker/microphone
- spotlight
- PIR (motion detection)

The PCB for this project is designed to fit in place of the original PCB, and reused it's mounting points.

The main camera is a RPi 5 module with a carrier camera.

This project replaces the PIR with a second camera, that is configured for object (specifically cat) recognition.This uses the Grove Vision AI v2 board, along with an original RPi camera.
This board can trigger a cat deterrent, such as a smell.

Photos of Yale disassembly 

KISS

# Specification 

  POE
  Compute module 5 basic
  12MP Raspberry Pi Camera Module 3, Standard
  
  Grove Vision AI Module V2
  Raspberry Pi basic camera OV5647-62 FOV Camera Module
for Raspberry Pi 3B+4B

  PIR or Grove board to trigger main Camera?
  
Todo: show  complete unit.

# Design Notes


Todo: show Schematic

# Images

![Yale Security Camera](:YaleCameraHousing.jpg)

![Grove Vision AI v2](:GroveVisionAIv2_1.png)
![Grove Vision AI v2](:GroveVisionAIv2_2.png)
![Grove Vision AI v2](:GroveVisionAIv2_3.png)

# PCB

The PCB has been produced using KiCAD 9.0

# Build Notes


# Operation Notes


# Applicable Links

https://core-electronics.com.au/guides/sensors/getting-started-with-the-grove-vision-ai-v2-power-efficient-object-detection/
https://wiki.seeedstudio.com/grove_vision_ai_v2_software_support/#-arduino-library-introduction-
Todo: show calculator kit sites

