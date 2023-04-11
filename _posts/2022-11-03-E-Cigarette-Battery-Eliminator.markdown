---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_E_Cigarette_Battery_Eliminator
title: E-Cigarette Battery Eliminator

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [jekyll, sample, example post]
# thumbnail image for post
img: ":BrotherPrinter2.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-10-30 08:11:06 +0900

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

This is a simple idea to re-use the batteries from a disposable E-cigarette and make a cheap and useful
battery eliminator. 

In this blog, I use the eliminator to power a
Brother label printer, and a Multimeter. 

The circuit uses a cheap chinese module that provides battery protection, a micro USB to charge 
the battery, and a boost circuit, so the unit can replace 6v to 12v batteries. The whole unit
costs a few pounds to make.

#### Typical E-Cigarette

![Typical E-Cigarette](:e-cigg.jpg){:data-align="center"}

The type of E Cigarette shown above does have an easiely recoverable battery, videos for
recovering these batteries are available on you tube. Other E-cigarettes may have batteries that are
more ecapsulated, and could prove dificult or hazardous to remove. If in any doubt, DON'T ATTEMPT IT!

![13350_battery](:13350_battery.jpg){:data-align="center"}

#### 13350 Battery recovered from e-cigarette
{:data-align="center"}

#### 3.7V 9V 5V 2A Adjustable Step Up 18650 Lithium Battery Charging Discharge Integrated Module

![Battery Control Module](:Module1.jpg){:data-align="center"}

The Module shown above is readily available on aliExpress, 

As the circuit/battery is permanently in circuit, an on/off switch is required, to maintain the battery power.

Two example installations are shown, for a Brother label printer, and a cheap Chinese multimeter.

[Battery Control Module](https://www.aliexpress.com/item/32976180245.html).

<!-- outline-end -->

#### Brother Printer Installation

The Brother label printer uses 6 AAA batteries, but can also be driven using an external power supply.
Using the external power connector and the battery eliminator makes the unit much easier to use
for creating the occassional label.
3-7V-9V-5V-2A-Adjustable-Step-Up
3.7V 9V 5V 2A Adjustable Step Up 18650 Lithium Battery Charging Discharge Integrated Module


![Complete Battery Eliminator](:BrotherPrinter1.jpg){:data-align="center"}

![Battery Eliminator Detail](:BrotherPrinter2.jpg){:data-align="center"}

![Exposed Battery Eliminator](:BrotherPrinter3.jpg){:data-align="center"}

#### Multimeter Installation

![Meter Battery Eliminator Fitting](:Meter1.jpg){:data-align="center"}

![Complete Meter Battery Eliminator Fitting](:Meter2.jpg){:data-align="center"}

## Applicable Links

[Battery Control Module](https://www.aliexpress.com/item/32976180245.html).


## 3.7V 9V 5V 2A Adjustable Step Up 18650 Lithium Battery Charging Discharge Integrated Module

 - Debug before use, the default output is about 9V
 - Input voltage 4.5-8V
 - The output voltage can be continuously adjusted from 4.3-27V (any voltage above 4.3V and below 27V can be output, and you can adjust the voltage counterclockwise by yourself)
 - The charging voltage is 4.2V and the charging current is up to 1A
 - Discharge current, the maximum output current of 2A should be calculated by yourself
 - Output reference maximum current 5V 1.4A , 9V 0.8A, 12V 0.6A
 - The quiescent current is about 0.5 mA
 - Overshoot protection Yes
 - Over-discharge protection No (it can also be said that there is, 2V cut off the boost but not block the output, the output still has 2V)
 - Cut-off boost 2V, depending on the situation, whether to add a protection board
 - Size 3.3X2.3X0.9
 - For example, the VIN+ terminal is connected to a 5V solar panel, and the BAT+ terminal can output 4.2V to charge a 3.7V 18650 battery
 - The OUT+ terminal can output an adjustable voltage, you can adjust how much you need
 - Can be used for multimeter modified lithium battery charging


