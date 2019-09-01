
<p align=center>
	<img alt="undefined" src="https://img.shields.io/github/license/thatguynikita/homeassistant-config.svg">
	<img src="https://img.shields.io/badge/hass-0.95.4-blue.svg">
	<img src="https://img.shields.io/badge/automations-11-purple.svg">
</p>

# Overview
Very minimalistic implementation of "smart" home based on [Home Assistant](https://www.home-assistant.io/) with Telegram integration. 
It won't cost you loads of money and will feed your curiosity about the current state of IoT.

# Hardware
| Device  | Qty | Home Assistant | Notes | 
| ------------- | :---: | ------------- | ------------- |
| [Raspberry Pi 3 Model B+](https://www.amazon.de/dp/B07BDR5PDW) | 1 | [HA on Docker](https://www.home-assistant.io/docs/installation/docker/) | Central home automation hub. Serves HA, [Mosquito](https://hub.docker.com/_/eclipse-mosquitto), Plex, Deluge, and many more | 
| [Raspberry Pi Zero W + camera](https://aliexpress.com/item/32831611503.html) | 1 | [Generic MJPEG IP Camera](https://www.home-assistant.io/components/mjpeg/) | Runs [motionEye](https://github.com/ccrisan/motioneye/wiki/Install-On-Raspbian) and reports motion detection via MQTT | 
| [Sonoff S20 Smart Socket](https://aliexpress.com/item/32823895149.html) | 1 | [Switch](https://www.home-assistant.io/components/switch/) / [Light Switch](https://www.home-assistant.io/components/light.switch/) | Flashed with [Sonoff-Tasmota](https://github.com/arendst/Sonoff-Tasmota/wiki/sonoff-S20) firmware. Controlled via MQTT | 
| [Amazon Echo Dot (3rd Gen)](https://www.amazon.de/dp/B07PHPXHQS) | 1 | [Alexa Smart Home Skill](https://www.home-assistant.io/components/alexa.smart_home/) | Bedroom speaker. Voice commands only | 
| [Google Home Mini](https://store.google.com/de/product/google_home_mini) | 1 | [Google Assistant](https://www.home-assistant.io/components/google_assistant/) | Kitchen speaker. Voice commands and casting music |  |
| [Google Chromecast (2nd Gen)](https://store.google.com/de/product/chromecast) | 1 | [Google Cast](https://www.home-assistant.io/components/cast/) | Living room TV. Mainly used for casting Plex | 
| [DIY Multisensor](https://www.youtube.com/watch?v=sVml02kP3DU) | 1 | [MQTT](https://www.home-assistant.io/components/mqtt/) | [NodeMCU](https://aliexpress.com/item/32665100123.html) based. Reports temperature, humidity ([DHT22](https://aliexpress.com/item/32769460765.html)), illuminance ([TSL2561](https://aliexpress.com/item/32905003264.html)) and detects motion ([PIR](https://aliexpress.com/item/32749737125.html)) | 

# Screenshots
![UI](images/lovelace.png?raw=true "Lovelace UI")

![UI](images/telegram.png?raw=true "Telegram bot")
