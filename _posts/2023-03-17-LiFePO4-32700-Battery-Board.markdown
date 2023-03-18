---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Torch_Rework
title: LiFePO4 support and development board

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


#### PCB as designed.

The PCB is designed as a 1.6mm thick board, double sided through hole plated.
Provision for SOT or axial resistors is provided.
The PCB is designed as a supplementary board to a main board with a micro-controller fitted.

![front view](:ESP32-CricketBatteryBoard115x90x55.jpg){:data-align="center"}

![back view](:ESP32-CricketBatteryBoard115x90x55_2.jpg){:data-align="center"}

#### PCB Housing.

The case is a standard Chinese 115x90x55 plastic box.
The battery board and main board are stacked in pillars, and the LiFePO4 battery is sandwiched between them.
This view of the case shows the 3.5mm soket fitted, which will later be used to charge the battery.

![case view](:ESP32-CricketBatteryBoard115x90x55_3.jpg){:data-align="center"}

#### PCB Populated.


#### Assembled Cricket Module.

![partial assembled view](:ESP32-CricketBatteryBoard115x90x55.jpg){:data-align="center"}

![full assembled view](:ESP32-CricketBatteryBoard115x90x55.jpg){:data-align="center"}


More Information on the Cricket2 project can be found in the relevant blog entries.

**Keep it simple**, the Cricket 2 modules are designed to have a minimum battery life of 3 months between recharges.
That is based on the module doing a transmission every ½ hour, so 2 x 24 x 92 transmission approx 3500 transmissions.


### Applicable Links

Link to project page [Battery Technology](https://www.batteryequivalents.com/32650-battery.html).
