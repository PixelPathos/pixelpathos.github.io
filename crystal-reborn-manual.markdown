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
The following is a list of all complications supported by Crystal Reborn. Icons will take on theme colour if **Colourful Icons** setting is turned off.

| Icon | Name | Side Meter | Data Field | Indicator | Notes |
| :--: | :--- | :--------: | :--------: | :-------: | :---- |
| ![Battery](/images/crystal-reborn/icons/battery@2x.png){: width="32"}![Battery low](/images/crystal-reborn/icons/battery-low@2x.png){: width="32"}![Battery critical](/images/crystal-reborn/icons/battery-critical@2x.png){: width="32"}![Battery charging](/images/crystal-reborn/icons/battery-charge@2x.png){: width="32"} | Battery | ✅ | ✅ | ✅ | Yellow warning shown at 20%. Red warning shown at 10%. Charging always shown in green, with charging symbol. Side meter and data field shows remaining battery % value.|
| " | Battery in Days | | ✅ | | Data field shows estimated remaining battery in days. |
| " | Battery (Hide %) | | ✅ | | Data field shows icon only. |
| ![Battery](/images/crystal-reborn/icons/battery-percent@2x.png){: width="32"}![Battery low](/images/crystal-reborn/icons/battery-percent-low@2x.png){: width="32"}![Battery critical](/images/crystal-reborn/icons/battery-percent-critical@2x.png){: width="32"}![Battery charging](/images/crystal-reborn/icons/battery-percent-charge@2x.png){: width="32"} | Battery (%) | | | ✅ | Indicator only. Charging always shown in green, with + symbol.|
| ![Steps](/images/crystal-reborn/icons/steps@2x.png){: width="32"} | Steps | ✅ | ✅ | | |
| ![Calories](/images/crystal-reborn/icons/calories@2x.png){: width="32"} | Calories | ✅ | ✅ | | Calories Goal for side meter is set manually via separate setting. |
| ![Active Calories](/images/crystal-reborn/icons/calories@2x.png){: width="32"} | Active Calories | ✅ | ✅ | | Estimate of active calories, based on gender, age, height, weight, and total calories. Side meter uses same Calories Goal as above. |
| ![Floors Climbed](/images/crystal-reborn/icons/floors-climbed@2x.png){: width="32"} | Floors Climbed | ✅ | ✅ | | Only supported by watches with barometers. |
| ![Active Minutes](/images/crystal-reborn/icons/active-minutes@2x.png){: width="32"} | Active Minutes | ✅ | ✅ | | |
| ![Current Weather Day](/images/crystal-reborn/icons/weather-day@2x.png){: width="32"}![Current Weather Night](/images/crystal-reborn/icons/weather-night@2x.png){: width="32"}etc. | Current Weather | | ✅ | | Most watches default to Garmin Weather as data source. OpenWeather is also supported, and is the only data source if Garmin Weather is not supported. See OpenWeather section for more details. <br><br>Temperature in **celcius** (metric) or **farenheit** (statute), depending on watch units setting. |
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

## Style

## Always On

Calories Goal

Hide Hours Leading Zero

Hide Seconds

App Version