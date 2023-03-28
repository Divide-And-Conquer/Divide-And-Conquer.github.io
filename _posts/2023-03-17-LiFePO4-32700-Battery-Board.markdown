---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Torch_Rework
title: LiFePO4 Battery -Support and Development Board

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":ESP32 - CricketBatteryBoard - Preview_1.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-03-17 15:17:00 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 
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

This board is principally designed to hold a 32700 sized battery in place, and make electrical contact with it.
For some reason battery holders for this battery are either not available, or are unsuitable.
The 32700 naming convention equate to 32mm diameter, and 70mm long (why extra zero?).

As a PCB was being manufactured for this purpose, I (as always) decided to make it multipurpose, by adding some
resistor signal conditioning, and by adding prototyping areas to the board.
The board does also have a cut-out to cater for a barrel-jack connector, to allow the battery to be charged in-situ.

![battery view](:32700 Battery.jpg){:data-align="center"}

<!-- outline-end -->


#### PCB as designed

The PCB is designed as a 1.6mm thick board, double sided through hole plated.
Provision for SOT or axial resistors is provided.
The PCB is designed as a supplementary board to a main board with a micro-controller fitted.

![front view](:ESP32-CricketBatteryBoard115x90x55.jpg){:data-align="center"}

![back view](:ESP32-CricketBatteryBoard115x90x55_2.jpg){:data-align="center"}

#### PCB Housing

The case is a standard Chinese 115x90x55 plastic box.
The battery board and main board are stacked in pillars, and the LiFePO4 battery is sandwiched between them.
This view of the case shows the 3.5mm soket fitted, which will later be used to charge the battery.

![case view](:ESP32-CricketBatteryBoard115x90x55_3.jpg){:data-align="center"}

#### Soldering Steps

The battery clips are difficult to solder. For a good contact with the battery
the clip needs to sit proud of the PCB. Fitting the clip and using a small wire to hold 
the clip in place when the board is upside down was found to make the soldering/assembly
process much easier, as the clip automatically fell into alignment.

The 3.5mm socket can be pre-fitted to the board, and soldered in-place, then it needs to
installed in it's socket, at the same time as the board is fitted on it's mounting screws.

![soldering clips 1](:ESP32-CricketBatteryBoard115x90x55_4.jpg){:data-align="left"}

![soldering clips 2](:ESP32-CricketBatteryBoard115x90x55_5.jpg){:data-align="center"}

![soldering clips 3](:ESP32-CricketBatteryBoard115x90x55_6.jpg){:data-align="right"}

#### Fitting Components

The -ve clip with it's spring does experience a lot of force when the battery is fitted, 
this causes it to bend, so a plastic filler is used to support the clip, and help mantain
pressure on the battery.

![partial assembled view](:ESP32-CricketBatteryBoard-Clip_support_1.jpg){:data-align="center"}

The pillars will then need to be fitted to support the main PCB.
A single 3.3V connection is made between the two boards.

The main board may optionally have an external DS18B20 external temperature probe.

Many of the batteries I have do not have a plastic sleeve, on these patteries I've
placed an insulating strip along the top of the battery to block contact with the underside
or the Cricket PCB.

![partial assembled view](:ESP32-CricketBatteryBoard-3_5mmConnector){:data-align="center"}

#### PCB Populated


#### Assembled Cricket Module

![partial assembled view](:ESP32-CricketBatteryBoard-Body1.jpg){:data-align="center"}

THe 3.3V connection attaches to the main board via its J4 connector,
0V = Pin 1, 3.3V = Pin 4.

The Spacers for the pillars between boards is ???

![full assembled view](:ESP32-CricketBatteryBoard-Body2.jpg){:data-align="center"}


More Information on the Cricket2 project can be found in the relevant blog entries.

**Keep it simple**, the Cricket 2 modules are designed to have a minimum battery life of 3 months between recharges.
That is based on the module doing a transmission every ½ hour, so 2 x 24 x 92 transmission approx 3500 transmissions.


### Applicable Links

Link to project page [Battery Technology](https://www.batteryequivalents.com/32650-battery.html).
