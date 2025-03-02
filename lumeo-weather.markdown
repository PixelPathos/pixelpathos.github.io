---
layout: default
title: Lumeo Weather Features
description: Lumeo, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /lumeo/weather
---
## OpenWeather Integration

### What is OpenWeather?
[OpenWeather](https://openweathermap.org/) is a popular third-party weather service. It is offered as an alternative to Garmin's own built-in weather service, as some users report that OpenWeather provides a more accurate forecast. OpenWeather also make additional data available, such as percentage cloud cover.

### Is OpenWeather available on my watch?
OpenWeather is available in Lumeo on almost all devices. Unfortunately, due to memory limitations, it is not available on some fēnix® 6 devices.

### How do I get started?
You will need a free OpenWeather API key, which you then need to enter in the "OpenWeather Key" box in Lumeo's settings in the Connect IQ app.

- **[Sign up for a free OpenWeather account]({{ openweather_sign_up_url }})** if you don't already have one. You will receive an account confirmation e-mail.
- **Click on the "Verify your email" button** in the confirmation e-mail. This will log you in to your OpenWeather account.
- **Click on the "API keys" tab.** You will see that an API key has already been generated for you. Copy, or write down this key.
- **In Lumeo's settings in the Connect IQ app, paste the key into the "OpenWeather Key" box, and save**. Note you can also do this in Garmin Express, but not currently on the watch itself. If you already have an OpenWeather key, you can skip the previous steps and use your existing key here instead.

### How will Lumeo use the OpenWeather API key?
Lumeo uses the "Current weather and forecast" service, and not "One Call" (at the moment).

Lumeo will fetch the latest weather via the internet when detects that the weather data it holds is older than 30 minutes. It will check the age of its data (before making a request) each time you wake your watch.

Additionally, each time you change settings, Lumeo will fetch the latest weather as soon as possible.

Lumeo can access the internet a maximum of once every 5 minutes. **This means you may see a delay, especially when activating OpenWeather for the first time.**

### How do I know OpenWeather is working?
Weather fields will now show a coloured dot, indicating the status of the OpenWeather data:

![Lumeo's Open Weather Status Indication](/images/lumeo-open-weather-status-indication.png)

| Dot Colour | Meaning |
| --- | --- |
| <span style="color:#666666">Grey</span> | No internet connection, or other request error. Ensure watch is paired with phone that has internet access. |
| <span style="color:#FFAA00">Yellow</span> | Unknown location, so can't request local weather. Lumeo initially requires a location from Garmin Weather, so ensure watch is paried with phone that has internet access. Lumeo will store the current location in case a live location is no longer available. |
| <span style="color:red">Red</span> | Invalid API Key. Check that you have entered a valid OpenWeather key correctly. |
| <span style="color:#FF5500">Orange</span> | Other HTTP error. |
| <span style="color:#00AAFF">Blue</span> | A request to OpenWeather has been queued, and will be made within the next 5 minutes. **If you have just set up OpenWeather, no data will be visible until the initial request has completed.** |
| <span style="color:white">White</span> | Successfully sent a request to OpenWeather; now awaiting response. |
| <span style="color:#00FF00">Green</span> | Up-to-date weather information successfully received. This indication will automatically disappear after 1 minute. |

## Advanced Weather

### What is Advanced Weather?
Advanced Weather replaces the usual middle dial (Dial 2) with a more detailed weather display. In addition to the current condition, and min/current/max temperatures, there are **3 new fields** (see above screenshot) where you can show additional information.

The feature is available on all watches, and works either with Garmin Weather, or OpenWeather.

### How do I enable Advanced Weather?
- Select one of the layouts that shows dials: Max Data, Dials and Graph, or Dials. You can do this via the ```Layout``` submenu in Lumeo's settings.
- Ensure that Dial 2 is set to Weather. Use the ```Data``` submenu for this.
- In the ```Weather``` submenu, turn on the ```Advanced Weather``` setting.
- That submenu also allows you to configure the 3 fields. Fields marked ```[GW]``` are only available when using Garmin Weather, while fields marked ```[OW]``` are only available when using OpenWeather.
