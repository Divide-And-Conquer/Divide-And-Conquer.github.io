---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_LiFePO4_Charger
title: LiFePO4 Charger

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":LiFePO4_Charger_1.jpg"
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

This project a charger for a LiFePO4 battery, it's main use
is to charge Cricket2 modudles, these have a 3.5mm socket which connects to the 
plug on the charger.

Two power sources are intended as the input to the charger, a mains driven 
generic "floating" PSU, or a solar panel.

The charger demonstrates the building something useful from nothing, or building from junk
principle.

![LiFePO4-Charger](:LiFePO4_Charger_5.jpg){:data-align="center"}

<!-- outline-end -->

### LiFePO4 Housing Assembly

The housing is a plastic box that used to house a drill bit.
The switch/voltmeter/Charger board/and other components were all items I had 
from previous projects.

Also the external 12V PSU is from a previous purchase.

![Schematic-LiFePO4-1](:LiFePO4_Charger_3.jpg){:data-align="center"}

![Schematic-LiFePO4-2](:LiFePO4_Charger_4.jpg){:data-align="center"}

### External PSU

![Schematic-LiFePO4-9](:LiFePO4_Charger_7.jpg){:data-align="center"}

### Schematic

![Schematic-LiFePO4-Charger](:Schematic-LiFePO4-Charger.jpg){:data-align="center"}

### Charger Module - 5A lithium battery step-down charging board LED power converter step-down module XL4015

![Schematic-LiFePO4-3](:Charger-Module.jpg){:data-align="center"}

https://www.aliexpress.com/item/32663793748.html


    Input: IN + input positive, IN- input negative

    Output way: OUT + output positive, OUT- output negative

    Input voltage: 4-38V

    Output voltage: 1.25-36V continuously adjustable

    Output current: adjustable, maximum 5A

    Output Power: 75W maximum

    Working temperature: -40 to + 85 degrees

    Operating frequency: 180KHz

    Conversion efficiency: up to 96%

    Short circuit protection: Yes (limit current 8A)

    Overtemperature protection: (automatically shut off the output after overtemperature)

    Input reverse polarity protection: None, (if necessary, please enter the string into the high current diode)

    Installation: four 3mm screws

    Module dimensions: length 51mm width 26mm height 15mm
