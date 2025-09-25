---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_DockerPi2
title: RPi - Node-red - MQTT - InfluxDB - Grafana

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Martin Rawson
# multiple category is not supported
category: jekyll
# multiple tag entries are possible
tags: [rpi, mqtt, iot]
# thumbnail image for post
img: ":Node-Red2.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2023-04-02 08:11:06 +0900

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

# Outline

<!-- outline-start -->

This project uses a RPi SBC (version 4 or later), Cricket 2 external sensors, and Tasmota mains pwer sockets.
It also requires the following software packages, Node-red, MQTT, InfluxDB, Grafana, Telegram.

The DockerPi2 server is a Raspberry Pi 400 Computer that connects to the Internet, and runs a set of programs which gather and process data from a number of sensors, and store the data, and render the data on one or more computers screens.

The Sensors transmit their data to the RPi using MQTT, the RPi runs a broker (server) that takes this data and passes it onto node-red for processing or forward transmission. Node-red allows for the creation of a number of dashboards to display the information:
```

```

![Crickets Monitor Page](:Node-Red1.jpg){:data-align="center"}
```

```


![Tasmota Plugs Page](:Node-Red2.jpg){:data-align="center"}
```

```

Node-red can be considered a toolbox which allows data to be processed, redirected, displayed and expanded (in the same way as a web-browser is expanded by plug-ins).

InfluxDB - Telegram

Grafana

Other software also runs on the RPi, like the mosquitto MQTT server, and RPi-connect for remote access.

<!-- outline-end -->

# Design Notes

Sensors providing data to node-red are primarily Cricket2 units, or smart sockets provided by living-bytes, these run
tasmota. These send json data via MQTT.

Node-red runs javascript, and also provides a graphical programming interface, these are used to create the interface,
custom javascript code handles the json unpacking/re-routing.

Todo: show Schematic

# Images

![Tasmota style Plug](:TASMOTA-WIFI-SmartSocket.png)

# Build Notes

This project originally ran on a RPi4, it now runs on a RPi400, this is a better suited to the project, as everything is in one place.

# Operation Notes

Todo: show Cricket2 or tasmota json strings

# Applicable Links

[home automation initial source](https://www.youtube.com/watch?v=a6mjt8tWUws)

[node-red main site](https://nodered.org/)

[local-bytes Smart Socket](https://www.mylocalbytes.com/products/smart-plug-pm)

