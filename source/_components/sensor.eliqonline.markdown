---
layout: page
title: "Eliqonline"
description: "Instructions how to integrate Eliqonline devices within Home Assistant."
date: 2015-07-11 0:15
sidebar: true
comments: false
sharing: true
footer: true
logo: eliq.png
ha_category: Sensor
ha_release: "0.10"
---


Integrate your [ELIQ Online](http://eliq.se) smart meter information into Home Assistant. To get an [acess token](https://my.eliq.se/user/settings/api) and the [Channel ID](https://my.eliq.se/user/settings/data), log in to your account.

To enable this sensor in your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
sensor:
  platform: eliqonline
  access_token: ACCESS_TOKEN
  name: Power consumption 
  channel_id: CHANNEL_ID
```

Configuration variables:

- **access_token** (*Required*): The Access Token for your account.
- **channel_id** (*Optional*): Channel ID of your device. Needed if you have more than one device.
- **name** (*Optional*): The name of the sensor, eg. the city.

For details please check the [API documentation](https://my.eliq.se/knowledge/sv-SE/49-eliq-online/299-eliq-online-api).

