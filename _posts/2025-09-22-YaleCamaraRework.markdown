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
tags: [camera, reuse, rework]
# thumbnail image for post
img: ":YaleCamaraReworkHousing.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2025-10-05 07:11:06 +0900

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

This project uses the case and various components from a All in one AW 01 Yale camera.
This camera was purchased on eBay with a known fault, essentially the Wi-fi did not work, 
and on investigation was seen to be unrealistic to repair.

The aim of this project is to see how much of the original broken Yale Camera can be reused and made useful, perhaps even returning it to being a full security working camera.

```
  What components from the Yale unit can be reused?
    - housing and mounting bracket
    - External PSU (not for this camera)
    - camera 
    - IR LEDs
    - speaker / siren
    - microphone
    - spotlight
    - Information LEDs
    - PIR (motion detection)
    - SD card
```

These components range in complexity, e.g. Leds should be simple to drive, but the camera would be very challenging to reuse.

One serious difficulty when building your own camera is finding a suitable housing, especially one that can be mounted externally. This is even more troublesome if the housing has to contain any extras (microphone/speaker/siren/PIR/second camera), the Yale camera unit has provision for these.

Sourcing a housing is difficult but you may also be able to obtain one on eBay as a damaged of failed unit.

![Yale Security Camera](:YaleCamaraReworkHousing.jpg){:data-align="center"}

# Hardware Investigation

The hardware in this unit is quite sophisticated, internally it contains 4 purpose built PCBs, these contain surface mount components and are connected using ribbon and discrete cables, .

The passive infrared (PIR) sensor is housed on its own PCB

![Yale Security Camera](:YaleCamaraElectronics_2.jpg){:data-align="center"}

The rest of the electronics is on 3 PCBS Linked with ribbon cables

![Yale Security Camera](:YaleCameraElectronics_1.jpg){:data-align="center"}

LED driver board provides spotlight, IR LEDs, Information LEDs

![LED driver board](:YaleCameraElectronics_3.jpg){:data-align="center"}

Main board provides CPU, Storage, Camera.

Interface board provides SD card, Wifi including Aerials

Todo: show Photos of Yale disassembly 

Todo: show complete unit

<!-- outline-end -->

# Specification / Design / KISS

  POE
  Compute module 5 basic
  12MP Raspberry Pi Camera Module 3, Standard
  
  Grove Vision AI Module V2
  Raspberry Pi basic camera OV5647-62 FOV Camera Module for Raspberry Pi 3B+4B?

  PIR or Grove board to trigger main Camera?

```
  ---> POE ---> RPi 5 POE hat ---> RPi 5 ---> Camera
                                       ---> Pico ---> spotlight
                                                 ---> AI camera 
                                                 ---> IR LEDs
                                                 ---> siren
                                                 ---> speaker/microphone
                                                 ---> PIR (motion detection)
```
                                             
# Design Notes

Other than the case itself, the first good candidate for reuse would appear to be the LED driver board (spotlight, IR LEDs, Information LEDs). these are driven via a ribbon cable, it will be necessary to identify the signals in the ribbon cable and to hook up to it.

The speaker / siren and microphone, but also appear to be good candidates.

The PIR sensor on its on the PCB is a possibility, but will require the signal interface to be determined.

A CPU module will have to be piggybacked onto a custom PCB.

The PCB for this project is designed to fit in place of the original PCB, and to use it's mounting points.

The main camera is a RPi 5 module with a carrier camera.

# Connector Pin assignments

These pin numbers are the original pin numbers/functions from the Yale Camera, the Wire colour column is not original but details the colours used with the new cables installed on the reworked camera.

```
LED PCB Connections
===================
| Pin No. | Function / Signal | Direction | Connected To (Board / MCU / Component) | Notes / Voltage |
| :-----: | :---------------- | :-------- | :------------------------------------- | :-------------- |
|    1    | —                 | —         | —                                      | —               |
|    2    | —             | —         | —                                      | —               |
|    3    | —             | —         | —                                      | —               |
|    4    | —             | —         | —                                      | —               |
|    5    | — GND             | —         | —                                      | —               |
|    6    | —             | —         | —                                      | —               |
|    7    | — GND             | —         | —                                      | —               |
|    8    | —               | —         | —                                      | —               |
|    9    | — 3.3V                | —         | —                                      | —               |
|    10   | —             | —         | —                                      | —               |
|    11   | — 3.3V                | —         | —                                      | —               |
|    12   | —             | —         | —                                      | —               |
|    13   | — GND             | —         | —                                      | —               |
|    14   | —              | —         | —                                      | —               |
|    15   | — GND             | —         | —                                      | —               |
|    16   | —                 | —         | —                                      | —               |
```

```
PIR PCB Connections
===================
| Pin No. | Function / Signal | Direction | Connected To (Board / MCU / Component) | Wire Colour     |
| :-----: | :---------------- | :-------- | :------------------------------------- | :-------------- |
|    1    | — 3.3V            | — Power   | —                                      | — Green         |
|    2    | — 0V              | — Power   | —                                      | — Yellow        |
|    3    | — 0V / 3V         | — Output  | — PIR Output                           | — Black         |
|    4    | —                 | —         | —                                      | — Red           |

```

## GPIO Assignments

  🟦 Outputs:
  
    GP3 → Spotlight
    GP4 → IR LEDs
    GP5 (PWM) → Speaker (siren, via amp)
    GP6 → PIR test LED
    GP7 → Info LED 1
    GP8 → Info LED 2
  
  🟩 Inputs:
  
    GP2 → PIR sensor
    GP9 → Test IN1 (toggles spotlight)
    GP10 → Test IN2 (toggles IR LEDs)
    GP11 → Test IN3 (toggles Info LED 1)
    GP12 → Test IN4 (toggles Info LED 2)
    GP13 → Test IN5 (PWM Siren)
  
  🔴 Power pins: 3.3V / 5V
  ⚫ Ground pins: GND

Todo: show Schematic

What is the control interface?

# Images


# PCB

The PCB has been produced using KiCAD 9.0
Todo: show PCBs

# Build Notes


# Operation Notes


# Applicable Links


[hd1080-all-in-one-indoor-outdoor-camera-white](https://yalehome.co.uk/hd1080-all-in-one-indoor-outdoor-camera-white)

# Photo Record

![Security Camera Breakdown 1](:SecurityCamera1.jpg){:data-align="center"}

![Security Camera Breakdown 2](:SecurityCamera2.jpg){:data-align="center"}

![Security Camera Breakdown 3](:SecurityCamera3.jpg){:data-align="center"}

![Security Camera Breakdown 4](:SecurityCamera4.jpg){:data-align="center"}

![Security Camera Breakdown 5](:SecurityCamera5.jpg){:data-align="center"}

![Security Camera Breakdown 6](:SecurityCamera6.jpg){:data-align="center"}


