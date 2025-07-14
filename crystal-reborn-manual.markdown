---
layout: default
title: Crystal Reborn Manual
description: Crystal Reborn, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /crystal-reborn/manual
---
![Crystal Reborn hero image](/images/crystal-reborn/hero-image.png)

The manual is currently a work-in-progress.

# Overview

![Crystal Reborn overview](/images/crystal-reborn/manual-overview.png){: width="960"}

# Settings menu

## Data

You can customise the data shown in the following areas of the watch face:
- Left Meter
- Right Meter
- Data Field 1
- Data Field 2
- Data Field 3
- Indicator 1
- Indicator 2
- Indicator 3

Not all complications are available in all areas. Not all complications are supported on a given device. If a given complication is not supported, the icon will be shown in grey without a value.

### Complications

The following is a list of all complications supported by Crystal Reborn. Icons will take on the theme colour if the [Colourful Icons](#colourful-icons) setting is turned off.

| Icon | Name | Side Meter | Data Field | Indicator | Description |
| :--: | :--- | :--------: | :--------: | :-------: | :---------- |
| ![Battery](/images/crystal-reborn/icons/battery@2x.png){: width="32"}![Battery low](/images/crystal-reborn/icons/battery-low@2x.png){: width="32"}![Battery critical](/images/crystal-reborn/icons/battery-critical@2x.png){: width="32"}![Battery charging](/images/crystal-reborn/icons/battery-charge@2x.png){: width="32"} | Battery | ✅ | ✅ | ✅ | Yellow warning shown at 20%. Red warning shown at 10%. Charging always shown in green, with charging symbol. Side meter and data field shows remaining battery % value.|
| " | Battery in Days | | ✅ | | Data field shows estimated remaining battery in days. |
| " | Battery (Hide %) | | ✅ | | Data field shows icon only. |
| ![Battery](/images/crystal-reborn/icons/battery-percent@2x.png){: width="32"}![Battery low](/images/crystal-reborn/icons/battery-percent-low@2x.png){: width="32"}![Battery critical](/images/crystal-reborn/icons/battery-percent-critical@2x.png){: width="32"}![Battery charging](/images/crystal-reborn/icons/battery-percent-charge@2x.png){: width="32"} | Battery (%) | | | ✅ | Indicator only. Charging always shown in green, with + symbol.|
| ![Steps](/images/crystal-reborn/icons/steps@2x.png){: width="32"} | Steps | ✅ | ✅ | | |
| ![Calories](/images/crystal-reborn/icons/calories@2x.png){: width="32"} | Calories | ✅ | ✅ | | [Calories Goal](#calories-goal) for side meter is set manually via separate setting. |
| ![Active Calories](/images/crystal-reborn/icons/calories@2x.png){: width="32"} | Active Calories | ✅ | ✅ | | Estimate of active calories, based on gender, age, height, weight, and total calories. Side meter uses same [Calories Goal](#calories-goal) as above. |
| ![Floors Climbed](/images/crystal-reborn/icons/floors-climbed@2x.png){: width="32"} | Floors Climbed | ✅ | ✅ | | Only supported by watches with barometers. |
| ![Active Minutes](/images/crystal-reborn/icons/active-minutes@2x.png){: width="32"} | Active Minutes | ✅ | ✅ | | |
| ![Current Weather Day](/images/crystal-reborn/icons/weather-day@2x.png){: width="32"}![Current Weather Night](/images/crystal-reborn/icons/weather-night@2x.png){: width="32"}etc. | Current Weather | | ✅ | | Most watches default to Garmin Weather as data source. OpenWeather is also supported, and is the only data source if Garmin Weather is not supported. See [OpenWeather](#openweather) section for more details. <br><br>Temperature in **celcius** (metric) or **farenheit** (statute), depending on watch units setting. |
| ![Humidity](/images/crystal-reborn/icons/humidity@2x.png){: width="32"} | Humidity | | ✅ | | Value from the same data source as weather. |
| ![Sunrise](/images/crystal-reborn/icons/sunrise@2x.png){: width="32"}![Sunset](/images/crystal-reborn/icons/sunset@2x.png){: width="32"}| Sunrise/Sunset | | ✅ | | Times taken from Garmin Weather if supported, otherwise calculated for current date and location. |
| ![Altitude](/images/crystal-reborn/icons/altitude@2x.png){: width="32"} | Altitude | | ✅ | | Altitude in **metres** (metric) or **feet** (statute), depending on watch units setting. |
| ![Pressure](/images/crystal-reborn/icons/pressure@2x.png){: width="32"} | Pressure | | ✅ | | Pressure shown in **millibars**. |
| ![Notifications None](/images/crystal-reborn/icons/notifications-none@2x.png){: width="32"}![Notifications](/images/crystal-reborn/icons/notifications@2x.png){: width="32"} | Notifications | | ✅ | ✅ | Dot shown if there are any unread notifications on the phone. |
| ![Heart Rate](/images/crystal-reborn/icons/hr@2x.png){: width="32"}![Heart Rate Live](/images/crystal-reborn/icons/hr-live@2x.png){: width="32"} | Heart Rate | | ✅ | | In high-power mode after tap/gesture, HR updates every second, and dot flashes.<br><br>In low-power mode (AOD on AMOLED, always-active on MIP), HR updates every minute, and dot is hidden.|
| " | Heart Rate Live 5s | | ✅ | | As above, except that when MIP devices enter low power/always-active mode, HR continues to update every second, for 5 seconds, before reverting to updates every minute. This is to save power in always-active mode.<br><br>AMOLED devices do not support per-second updates when AOD is active. |
| ![Weekly Run Distance](/images/crystal-reborn/icons/run-distance@2x.png){: width="32"} | Weekly Run Distance | | ✅ | | Distance shown in **kilometres** (metric) or **miles** (statute), depending on watch units setting. |
| ![Weekly Bike Distance](/images/crystal-reborn/icons/bike-distance@2x.png){: width="32"} | Weekly Bike Distance | | ✅ | | Distance shown in **kilometres** (metric) or **miles** (statute), depending on watch units setting. |
| ![Recovery Time](/images/crystal-reborn/icons/recovery-time@2x.png){: width="32"} | Recovery Time | ✅ | ✅ | | Maximum value is 4 days, used as maximum value on side meter. |
| ![Stress](/images/crystal-reborn/icons/stress@2x.png){: width="32"} | Stress | ✅ | ✅ | | Unitless value from 0 to 100. |
| ![Body Battery](/images/crystal-reborn/icons/body-battery@2x.png){: width="32"} | Body Battery | ✅ | ✅ | | If current value is not available, an historical value up to 10 minutes old will be shown. |
| ![Run VO2 Max](/images/crystal-reborn/icons/vo2-max-run@2x.png){: width="32"} | Run VO2 Max | ✅ | ✅ | | |
| ![Bike VO2 Max](/images/crystal-reborn/icons/vo2-max-bike@2x.png){: width="32"} | Bike VO2 Max | ✅ | ✅ | | |
| ![Oxygen Saturation](/images/crystal-reborn/icons/o2-sat@2x.png){: width="32"} | Oxygen Saturation | ✅ | ✅ | | |
| ![Respiration Rate](/images/crystal-reborn/icons/resp-rate@2x.png){: width="32"} | Respiration Rate | | ✅ | | |
| ![Solar Input](/images/crystal-reborn/icons/solar-charge@2x.png){: width="32"} | Solar Charge | | ✅ | | Solar watches only. |
| ![Thermometer](/images/crystal-reborn/icons/temperature@2x.png){: width="32"} | Thermometer | | ✅ | | As measured by the watch, unrelated to weather forecast temperature. |
| ![Wheelchair Pushes](/images/crystal-reborn/icons/wheelchair-pushes@2x.png){: width="32"} | Wheelchair Pushes | ✅ | ✅ | | In wheelchair mode only. |
| ![Distance](/images/crystal-reborn/icons/distance@2x.png){: width="32"} | Distance | | ✅ | | Distance shown in **kilometres** (metric) or **miles** (statute), depending on watch units setting. |
| ![Alarms](/images/crystal-reborn/icons/alarms@2x.png){: width="32"} | Alarms | | ✅ | ✅ | Icon shown in grey if no alarms are set. |
| ![Bluetooth Disconnected](/images/crystal-reborn/icons/bluetooth-none@2x.png){: width="32"}![Bluetooth](/images/crystal-reborn/icons/bluetooth@2x.png){: width="32"} | Bluetooth | | | ✅ | Whether Bluetooth connection to phone is available. |
| ![Bluetooth Disconnected](/images/crystal-reborn/icons/bluetooth-none@2x.png){: width="32"}![Bluetooth](/images/crystal-reborn/icons/bluetooth@2x.png){: width="32"}![Notifications](/images/crystal-reborn/icons/notifications@2x.png){: width="32"} | Bluetooth/Notifications | | | ✅ | If Bluetooth is disconnected, shows grey Bluetooth icon.<br><br>If Bluetooth is connected and there are no notifications, shows coloured Bluetooth icon.<br><br>If Bluetooth is connected and there are notifications, shows notifications icon with dot. |

## Colour

### Theme

The theme colour changes the base colour of major elements of the watch face: the time, the side meters and the move bar. If the [Colourful Icons](#colourful-icons) setting is turned off, then all icons will take on the theme colour.

Theme colours either have a dark (black) or light (white) background. In order to protect battery life, AMOLED devices only support dark themes.

| ![Dark Theme](/images/crystal-reborn/dark-theme.png){: width="125"} | ![Dark Theme AOD](/images/crystal-reborn/dark-theme-aod.png){: width="125"} | ![Light Theme (MIP only)](/images/crystal-reborn/light-theme-mip-only.png){: width="125"} |
| :-: | :-: | :-: | :-: |
| Dark Theme | Dark Theme AOD | Light Theme (MIP only) |

### Colour Gradients

Show a colour gradient on the time, and for AMOLED devices, on the side meters and move bar.

| ![Colour Gradients On (AMOLED)](/images/crystal-reborn/colour-gradients-on-amoled.png){: width="125"} | ![Colour Gradients Off (AMOLED)](/images/crystal-reborn/colour-gradients-off-amoled.png){: width="125"} | ![Colour Gradients On (MIP)](/images/crystal-reborn/colour-gradients-on-mip.png){: width="125"} | ![Colour Gradients Off (MIP)](/images/crystal-reborn/colour-gradients-off-mip.png){: width="125"} |
| :-: | :-: | :-: | :-: |
| Colour Gradients On (AMOLED) | Colour Gradients Off (AMOLED) | Colour Gradients On (MIP) | Colour Gradients Off (MIP) |

### Colourful Icons

If turned **on**, each icon will be assigned a specific colour to make it stand out. If turned **off**, all icons will take on the theme colour.

### Hours Colour

There are three possible options for the colour of the hours digits:

| Option | Description |
| ------ | ----------- |
| (From Theme) | The hours digits take on the colour of the selected theme. |
| Mono Highlight | The hours digits are shown in monochrome (greyscale), with **maximum contrast** relative to the background i.e. in white for a dark theme, or in black for a light theme. |
| Mono | The hours digits are shown in monochrome (greyscale), with **medium contrast** relative to the background i.e. in light grey for a dark theme, or in dark grey for a light theme. |

### Minutes Colour

As above, except affecting the minutes digits.

## Style

### Meter Style

The settings controls the appearance of the segments for both side meters.

| Option | Description |
| ------ | ----------- |
| All Segments | Both the filled (theme colour) and unfilled (grey) segments of the meter are shown individually, with smaller gaps between the minor divisions, and larger gaps between the major divisions. |
| All Segments (Merged) | All filled segments are merged into a single segement, and all unfilled segments are merged into a single segment. |
| Filled Segments | Only the filled segments are shown, as individual segments. Unfilled segments are completely hidden. |
| Filled Segments (Merged) | Only the filled segments are shown, merged into a single segment. Unfilled segments are completely hidden.|
| Hidden | All segments are completely hidden. |

### Meter Digits Style

This setting controls which values are shown for both side meters.

| Option | Description |
| ------ | ----------- |
| Current/Target | Both current and target (goal) values are shown. |
| Current | Only current value is shown. Note that the target value is always hidden in AOD mode. |
| Hidden | Both values are hidden; only the icon is shown. |

### Move Bar Style

This setting controls the appearance of the move bar.

| Option | Description |
| ------ | ----------- |
| All Segments | Both filled (theme colour) and unfilled (grey) segments are shown. |
| Filled Segments | Only the filled segments are shown. Note that if no segments are filled, then this option will result in the move bar being completely invisible. |
| Hidden | Move bar is completely hidden. |

## Always On

Always On Display (AOD) is a low power mode supported by AMOLED devices only, where the watch face shows a simplified display in order to save battery. Always On needs to be enabled in the general settings menu on the watch, or else the watch will turn off the display after a period of inactivity, instead of entering Always On.

The general settings menu also allows you to change the timeout (delay) before the watch enters Always On mode.

In Crystal Reborn, you can independently control which elements are shown in Always On mode:

- Meters
- Meter Digits
- Data Fields
- Indicators
- Move Bar

Note that in Always On mode, in order to save battery, the side meter and move bar segments are made thinner, the goal values for the side meters are hidden, and seconds are hidden.

### Calories Goal

This is used as the goal (target) value when either **Calories** or **Active Calories** complications are shown in a side meter - the same value is used for both. While the default is 2,000 calories, this should not be interpreted as any kind of recommendation.

### Hide Hours Leading Zero

When turned on, if the hours begin with a zero, it will be hidden. Here is how the the setting affects the time display, in conjunction with the 12-/24-hour time format setting:

| Time | Leading Zero Off (12-hour) | Leading Zero On (12-hour) | Leading Zero Off (24-hour) | Leading Zero On (24-hour) |
| --- | :-: | :-: | :-: | :-: |
| 6am | **6**00 A | **06**00 A | **6**00 | **06**00 |
| noon | **12**00 P | **12**00 P | **12**00 | **12**00 |
| 6pm | **6**00 P | **06**00 P | **18**00 | **18**00 |
| midnight | **0**00 A | **00**00 A | **0**00 | **00**00 |

The 12-/24-hour time format setting can be changed via the general settings menu on the watch. There is no separate setting for this in Crystal Reborn.

### Hide Seconds

If turned on, the seconds display will be hidden, and the move bar will extend to fill the space.

Note that in Always On mode, seconds are always hidden.

### App Version

The version number of Crystal Reborn currently running on the watch. This is useful for checking whether your watch has updated to the latest version, in case you are waiting for a new feature or fix.

# OpenWeather

## What is OpenWeather?
[OpenWeather](https://openweathermap.org/) is a popular third-party weather service. It is offered as an alternative to Garmin's own built-in weather service, as some users report that OpenWeather provides a more accurate forecast.

## How do I get started?
You will need a free OpenWeather API key, which you then need to enter in the "OpenWeather Key" box in Crystal Reborn's settings in the Connect IQ app.

- **[Sign up for a free OpenWeather account]({{ openweather_sign_up_url }})** if you don't already have one. You will receive an account confirmation e-mail.
- **Click on the "Verify your email" button** in the confirmation e-mail. This will log you in to your OpenWeather account.
- **Click on the "API keys" tab.** You will see that an API key has already been generated for you. Copy, or write down this key.
- **In Crystal Reborn's settings in the Connect IQ app, paste the key into the "OpenWeather Key" box, and save**. Note you can also do this in Garmin Express, but not currently on the watch itself. If you already have an OpenWeather key, you can skip the previous steps and use your existing key here instead.

## How will Crystal Reborn use the OpenWeather API key?
Crystal Reborn uses the "Current weather and forecast" service, and not "One Call" (at the moment).

Crystal Reborn will fetch the latest weather via the internet when detects that the weather data it holds is older than 30 minutes. It will check the age of its data (before making a request) each time you wake your watch.

Additionally, each time you change settings, Crystal Reborn will fetch the latest weather as soon as possible.

Crystal Reborn can access the internet a maximum of once every 5 minutes. **This means you may see a delay, especially when activating OpenWeather for the first time.**

## How do I know OpenWeather is working?
The weather field will now show a coloured dot, indicating the status of the OpenWeather data:

![Crystal Reborn's OpenWeather Status Indication](/images/crystal-reborn/openweather-status-indication.png){: width="239"}

| Dot Colour | Meaning |
| --- | --- |
| <span style="color:#666666">Grey</span> | No internet connection, or other request error. Ensure watch is paired with phone that has internet access. |
| <span style="color:#FFAA00">Yellow</span> | Unknown location, so can't request local weather. Crystal Reborn initially requires a location from Garmin Weather, so ensure watch is paired with a phone that has internet access. Crystal Reborn will store the current location in case a live location is no longer available. |
| <span style="color:red">Red</span> | Invalid API Key. Check that you have entered a valid OpenWeather key correctly. |
| <span style="color:#FF5500">Orange</span> | Other HTTP error. |
| <span style="color:#00AAFF">Blue</span> | A request to OpenWeather has been queued, and will be made within the next 5 minutes. **If you have just set up OpenWeather, no data will be visible until the initial request has completed.** |
| <span style="color:white">White</span> | Successfully sent a request to OpenWeather; now awaiting response. |
| <span style="color:#00FF00">Green</span> | Up-to-date weather information successfully received. This indication will automatically disappear after 1 minute. |