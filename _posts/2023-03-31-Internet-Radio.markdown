---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Internet-Radio
title: Internet Radio

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [pi-zero, radio, reuse]
# thumbnail image for post
img: ":Kitchen_Radio_1.jpg"
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

### Outline

![Internet Radio 1](:Kitchen_Radio_1.jpg){:data-align="center"}

<!-- outline-start -->

Two Internet Radios have been made, they use the RPi Zero W to access the Internet, and I2S 'HATs' to provide Audio output.

![Internet Radio 4](:Kitchen_Radio_4.jpg){:data-align="center"}


![Internet_Radio](:Internet_Radio.jpg){:data-align="center"}

#### Internet Radio 
{:data-align="center"}



The unit is powered from a USB power adapter.

The Internet Radios are housed in PowerSafer cases, these cases are another product that has been upcycled.
The plastic case, and it's internal PCB containing an IR detector, and integrated switch and two LEDs have been used by the Radio.
The external mains plug and socket have been reused to make mains extension leads.
I could not find a use for the main PCB.

I2S is used to provide the audio output from the RPi, with the kitchen radio an Adafruit Preamp board is used to power the Bose external amp/speaker (another street find/freebie). With the Study Radio a Pimeroni Pirate Radio module was used, this drives a speaker directly.

The software used is the Pirate Radio provided by Pimeroni. The Infra-Red receiver code was lifted directly from LibraElec this has the flexibility that any OR remote can be made to work with it. I use some TV remotes purchased from poundland.

A small python program runs which calls the LibraElec software, and also the front mounted push-button, to allow the unit to be shut down.

<!-- outline-end -->

![Internet Radio 2](:Kitchen_Radio_2.jpg){:data-align="center"}

### Kitchen Radio

![Internet Radio 3](:Kitchen_Radio_3.jpg){:data-align="center"}

### Study Radio

![Internet Radio 5](:Kitchen_Radio_5.jpg){:data-align="center"}

### Software

The Stations list is held in /home/pi/.config/vlc/playlist.m3u

  sudo nano /home/pi/.config/vlc/playlist.m3u in a terminal, 
  adding the URLs for the stations, one per line, and then pressing control and x, then y, then enter to save and exit. 

If a station cannot be found the Radio will try to play the next station in the list.

The codes for the remote are held in

Software is present for the unit to learn a new remote.

The unit can be monitored/controlled remotely on a web-browser using VLC.

How do I log into the VLC stream from a PC
 
  http://KitchenRadio.local:8080 or  http://StudyRadio.local:8080

  leave username blank and use password raspberry

