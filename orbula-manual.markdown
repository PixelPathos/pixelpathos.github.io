---
layout: default
title: Orbula Manual
description: Orbula, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /orbula/manual
app_name: Orbula
---
![Orbula hero image](/images/orbula/hero-image.png)

# Versions

{% capture versions %}
{% include gpay-kpay-versions.md
    app_name="Orbula"
    gpay_store_url=site.orbula_store_url
    kpay_store_url=site.orbula_kpay_store_url
    kpay_trial_hours=site.orbula_kpay_trial_hours
%}
{% endcapture %}

{{ versions | markdownify }}

# Overview

![Orbula overview](/images/orbula/overview@2x.png){: width="960"}

Orbula is designed to be highly customisable. Here are some of the things you can change:
- The [number of "satellite" dials](#layout) from 3 to 6;
- The [position of the time dial](#time-position);
- The [theme](#theme-colour), [background](#background) and [icon](#colourful-icons) colours;
- The time format ([12/24 hour](#time-format), and [leading zero](#show-hours-leading-zero));
- The font and colour of the [hours](#hours-fonthours-colour), [separator](#separator-fontseparator-colour) and [minutes](#minutes-fontminutes-colour), and the [type of separator](#separator);
- The data shown on the side meters, dials and line meter;
- The icons;
- The [brightness of the always-on display](#always-on) (AMOLED only).

# Settings menu

{% capture settings-menu-manual-pages %}
{% include settings-menu-manual-pages.md %}
{% endcapture %}

{{ settings-menu-manual-pages | markdownify }}

## Appearance

| | Time + 3 Dials | Time + 4 Dials | Time + 5 Dials | Time + 6 Dials |
| :- | :-: | :-: | :-: | :-: |
| **Top** | ![Time + 3 Dials, Top](/images/orbula/3-dials-top.png){: width="125"} | ![Time + 4 Dials, Top](/images/orbula/4-dials-top.png){: width="125"} | ![Time + 5 Dials, Top](/images/orbula/5-dials-top.png){: width="125"} | ![Time + 6 Dials](/images/orbula/6-dials.png){: width="125"} 
| **Right** | ![Time + 3 Dials, Right](/images/orbula/3-dials-right.png){: width="125"} | ![Time + 4 Dials, Right](/images/orbula/4-dials-right.png){: width="125"} | ![Time + 5 Dials, Right](/images/orbula/5-dials-right.png){: width="125"} | |
| **Bottom** | ![Time + 3 Dials, Bottom](/images/orbula/3-dials-bottom.png){: width="125"} | ![Time + 4 Dials, Bottom](/images/orbula/4-dials-bottom.png){: width="125"} | ![Time + 5 Dials, Bottom](/images/orbula/5-dials-bottom.png){: width="125"} | |
| **Left** | ![Time + 3 Dials, Left](/images/orbula/3-dials-left.png){: width="125"} | ![Time + 4 Dials, Left](/images/orbula/4-dials-left.png){: width="125"} | ![Time + 5 Dials, Left](/images/orbula/5-dials-left.png){: width="125"} | |

### Layout

Number of satellite dials (the time dial is always visible). Options are:

- Time + 3 Dials
- Time + 4 Dials (default)
- Time + 5 Dials
- Time + 6 Dials

### Time Position

Set the position of the time dial. When 6 satellite dials are shown on round watches, time is always central regardless of this setting. Options are:

- Top
- Right
- Bottom
- Left (default)

### Theme Colour

The theme colour is used for the "accent" colour on the watch face e.g. for the day of the week, the minutes and seconds, and the various meters and dials. The [background](#background) colour is also chosen based on the theme colour. Choose from one of 16 possible colours.

### Background

There are 5 different gradient backgrounds available. The **Auto** setting chooses the most suitable background for the current theme colour. The **None** setting turns off the background (black). Some MIP watches render only the central part of the background, using fewer colours, due to memory constraints.

### Draw Gradients

Controls whether colour gradients are used to render the time.

### Colourful Icons

| ![Colourful Icons On](/images/orbula/colourful-icons-on.png){: width="125"} | ![Colourful Icons Off](/images/orbula/colourful-icons-off.png){: width="125"} |
| :-: | :-: |
| Colourful Icons **On** (default) | Colourful Icons **Off** |

If turned on, complication icons are shown in distinct colours e.g. blue for body battery, purple for floors climbed. If turned off, all icons are shown in the [theme colour](#theme-colour).

Some icons, like the weather, are always shown in the theme colour; other icons, like the battery, are always shown in a distinct colour, regardless of this setting.

## Always On

This sub-menu is only available on AMOLED devices, and affects the display when always on mode is enabled and active.

### Brightness

The watch already dims the display when in always on mode; Orbula dims the display further. This setting controls the overall brightness of the watch face. 100% is the watch's default always on brightness. Default is 50%.

### Time Brightness

Orbula allows separate control of the time brightness in always on mode e.g. to allow the time to stand out from the rest of the watch face. Default is 80%.

## Time

| --- | :- |
| ![Default Time Display](/images/orbula/time-default.png){: width="91"} | White semibold hours, white semibold bar separator, theme-colour light minutes (default). |
| ![Time Variant 1](/images/orbula/time-variant-1.png){: width="91"} | Theme-colour bold hours and minutes, white bold colon separator. |
| ![Time Variant 2](/images/orbula/time-variant-2.png){: width="91"} | White bold hours, no separator, theme-colour extralight minutes. |
| ![Time Variant 3](/images/orbula/time-variant-3.png){: width="91"} | White semibold hours, grey extralight colon separator, grey light minutes. |

| Time | Leading Zero Off<br>12-hour | Leading Zero On<br>12-hour | Leading Zero Off<br>24-hour | Leading Zero On<br>24-hour<br>(Military Time) |
| --- | :-: | :-: | :-: | :-: |
| 6am | **6**00 | **06**00 | **6**00 | **06**00 |
| noon | **12**00 | **12**00 | **12**00 | **12**00 |
| 6pm | **6**00 | **06**00 | **18**00 | **18**00 |
| midnight | **0**00 | **00**00 | **0**00 | **00**00 |

### Time Format

Controls whether the time is shown in 12-hour or 24-hour format. The **Auto** setting (default) means that Orbula will respect the general Time Format setting on your watch. Setting **12 Hour** or **24 Hour** will override the general watch setting. See also [Show Hours Leading Zero](#show-hours-leading-zero).

### Hours Font/Hours Colour

Control the appearance of the hours. Options for the font are, from thinnest to thickest:

- ExtraLight
- Light
- Semibold
- Bold

Options for the colour are:

- Theme Colour
- Grey
- White

If [Draw Gradients](#draw-gradients) is turned on, a colour gradient will be shown.

### Separator

Controls the separator between the hours and the minutes. Options are:

- **None** (no separator: recommend choosing different fonts for hours and minutes)
- **\|** (bar, default)
- **:** (colon)

### Separator Font/Separator Colour

Control the appearance of the separator.

### Minutes Font/Minutes Colour

Control the appearance of the minutes.

### Show Hours Leading Zero

If the hour number would be a single digit, add a zero before that digit. Default is off.

### Show Seconds

Default is on. Note that AMOLED devices will always hide the seconds in always on mode, regardless of this setting.

## Side Meters

The **Left Side Meter** and **Right Side Meter** settings control the data visible on each side of the time. Only values that have a goal (e.g. steps goal) or maximum (e.g. 100% for battery) can be shown here. The numerical value is shown above each meter. Options are:

| Icon | Name | Notes |
| :-: | :- | :- |
| | Off | Hide the meter. |
| ![Battery (%)](/images/orbula/icon-battery.png){: width="32"} | Battery (%) | Current battery level in %. |
| ![Battery (Days)](/images/orbula/icon-battery.png){: width="32"} | Battery (Days) | Current battery level, with estimated remaining battery life in days or hours. |
| ![Steps](/images/orbula/icon-steps.png){: width="32"}| Steps | |
| ![Calories](/images/orbula/icon-calories.png){: width="32"} | Calories | Calories burnt for the current day. Calories goal is set manually using the [Calories Goal](#calories-goal) setting. |
| ![Active Calories](/images/orbula/icon-calories.png){: width="32"} | Active Calories | An estimate of active calories burnt for the current day, based on gender, age, height, weight, and total calories. Active calories goal is set manually using the same [Calories Goal](#calories-goal) setting as above. |
| ![Floors Climbed](/images/orbula/icon-floors-climbed.png){: width="32"} | Floors Climbed | Only supported by watches with barometers. |
| ![Active Minutes (Weekly)](/images/orbula/icon-active-minutes.png){: width="32"} | Active Minutes (Weekly) | |
| ![Recovery Time](/images/orbula/icon-recovery-time.png){: width="32"} | Recovery Time | Maximum value is 96 hours (4 days). |
| ![Stress](/images/orbula/icon-stress.png){: width="32"} | Stress | |
| ![Body Battery](/images/orbula/icon-body-battery.png){: width="32"} | Body Battery | If a current value is not available, an historical value up to 10 minutes old will be shown. |
| ![Run VO2 Max](/images/orbula/icon-run-vo2-max.png){: width="32"} | Run VO2 Max | Maximum value is 60. |
| ![Bike VO2 Max](/images/orbula/icon-bike-vo2-max.png){: width="32"} | Bike VO2 Max | Maximum value is 60. |
| ![Oxygen Saturation](/images/orbula/icon-o2-sat.png){: width="32"} | Oxygen Saturation | |
| ![Solar Input](/images/orbula/icon-solar-input.png){: width="32"} | Solar Input | Solar watches only. |
| ![Wheelchair Pushes](/images/orbula/icon-wheelchair-pushes.png){: width="32"} | Wheelchair Pushes | In wheelchair mode only. |

## Dials

Up to 6 dials may be shown in addition to the time dial, depending on the selected [layout](#layout).

| Dial | Name | Notes |
| :-: | :- | :- |
| ![Battery (%)](/images/orbula/dial-battery-percent@2x.png){: width="72" style="max-width: none;"} | Battery (%) | Current battery level in %. |
| ![Battery (Days)](/images/orbula/dial-battery-days@2x.png){: width="72"} | Battery (Days) | Current battery level, with estimated remaining battery life in days or hours. |
| ![Steps](/images/orbula/dial-steps@2x.png){: width="72"} | Steps | |
| ![Steps (Daily)](/images/orbula/dial-steps-daily@2x.png){: width="72"} | Steps (Daily) | Each bar represents the number of steps on that day. The leftmost bar is one week ago, the rightmost <span style="color:white">white</span> bar is today. A <span style="color:red">theme-coloured</span> bar means the goal was achieved that day; otherwise, the bar is <span style="color:#808080">grey</span>, and the thin <span style="color:#808080">grey</span> line shows the goal value. |
| ![Calories](/images/orbula/dial-calories@2x.png){: width="72"} | Calories | Calories goal is set manually using the [Calories Goal](#calories-goal) setting. |
| ![Calories (Daily)](/images/orbula/dial-calories-daily@2x.png){: width="72"} | Calories (Daily) | Calories goal is set manually using the [Calories Goal](#calories-goal) setting, and is used for all days |
| ![Active Calories](/images/orbula/dial-active-calories@2x.png){: width="72"} | Active Calories | An estimate of active calories burnt for the current day, based on gender, age, height, weight, and total calories. Active calories goal is set manually using the same [Calories Goal](#calories-goal) setting as above. |
| ![Floors Climbed](/images/orbula/dial-floors-climbed@2x.png){: width="72"} | Floors Climbed |  |
| ![Floors Climbed Daily](/images/orbula/dial-floors-climbed-daily@2x.png){: width="72"} | Floors Climbed (Daily) |  |
| ![Active Minutes (Weekly)](/images/orbula/dial-active-minutes@2x.png){: width="72"} | Active Minutes (Weekly) |  |
| ![Weather](/images/orbula/dial-weather@2x.png){: width="72"} | Weather | Current forecast temperature and condition. Dial min/max temperatures are for the whole day (Garmin Weather) or the remainder of the day (OpenWeather). Temperature is in degrees **celcius** (metric) or **farenheit** (statute), based on the Temperature Units setting on your watch. |
| ![Weather (Min/Max)](/images/orbula/dial-weather-min-max@2x.png){: width="72"} | Weather (Min/Max) | Current forecast temperature and condition, plus min/max temperatures for the whole day (Garmin Weather) or the remainder of the day (OpenWeather). Temperatures are in degrees **celcius** (metric) or **farenheit** (statute), based on the Temperature Units setting on your watch. |
| ![Humidity](/images/orbula/dial-humidity@2x.png){: width="72"} | Humidity |  |
| ![Sunrise/Sunset](/images/orbula/dial-sunrise-sunset@2x.png){: width="72"} | Sunrise/Sunset | Time and type of next "sun event" (sunrise or sunset). Dial represents time between previous and next sun events e.g. how far through daytime you are.  |
| ![Sunrise/Sunset (Today)](/images/orbula/dial-sunrise-sunset-today@2x.png){: width="72"} | Sunrise/Sunset (Today) | Sunrise time (top), sunset time (bottom) and next "sun event" icon (sunrise or sunset). Time of next sun event today is shown in <span style="color:white">white</span>. Bar represents the current 24 hours: <span style="color:#808080">grey</span> is night, <span style="color:#ffaa00">yellow</span> is day, and <span style="color:white">white</span> pointer is the current time.|
| ![Altitude](/images/orbula/dial-altitude@2x.png){: width="72"} | Altitude | Current altitude in **m** (metric) or **ft** (statute), based on the Elevation Units setting on your watch. |
| ![Altitude (Graph)](/images/orbula/dial-altitude-graph@2x.png){: width="72"} | Altitude (Graph) | Each of the 12 bars represent the min and max altitude for a 5-minute period by default i.e. 1 hour total. The graph duration can be changed using the [Graph Duration](#graph-duration) setting. A <span style="color:#808080">grey</span> circle is shown if no value is available for that time period. |
| ![Pressure](/images/orbula/dial-pressure@2x.png){: width="72"} | Pressure | Current pressure in **mb/hPa**, **inHg** or **mmHg**, based on the [Pressure Units](#pressure-units) setting. |
| ![Pressure (Graph)](/images/orbula/dial-pressure-graph@2x.png){: width="72"} | Pressure (Graph) | Pressure in **mb/hPa**, **inHg** or **mmHg**, based on the [Pressure Units](#pressure-units) setting. The graph duration can be changed using the [Graph Duration](#graph-duration) setting. |
| ![Notifications](/images/orbula/dial-notifications@2x.png){: width="72"} | Notifications | Number of unread phone notifications. Icon is shown in <span style="color:#808080">grey</span> if there are no notifications. |
| ![Heart Rate](/images/orbula/dial-heart-rate@2x.png){: width="72"} | Heart Rate | The minimum value is your resting heart rate, or zone 1 minimum if not available. The maximum value is zone 5 maximum. Heart rate zones are taken from your user profile. |
| ![Heart Rate (Graph)](/images/orbula/dial-heart-rate-graph@2x.png){: width="72"} | Heart Rate (Graph) | The graph duration can be changed using the [Graph Duration](#graph-duration) setting. |
| ![Heart Rate (Zones)](/images/orbula/dial-heart-rate-zones@2x.png){: width="72"} | Heart Rate (Zones) | The 5 heart rate zones (<span style="color:#aaaaaa">Z1</span>, <span style="color:#00aaff">Z2</span>, <span style="color:#00ff00">Z3</span>, <span style="color:#ffaa00">Z4</span>, <span style="color:red">Z5</span>) are taken from your user profile. |
| ![Weekly Run Distance](/images/orbula/dial-weekly-run-distance@2x.png){: width="72"} | Weekly Run Distance | Distance in **km** (metric) or **mi** (statute), based on the Distance Units setting on your watch. |
| ![Weekly Bike Distance](/images/orbula/dial-weekly-bike-distance@2x.png){: width="72"} | Weekly Bike Distance | Distance in **km** (metric) or **mi** (statute), based on the Distance Units setting on your watch. |
| ![Recovery Time](/images/orbula/dial-recovery-time@2x.png){: width="72"}| Recovery Time | Maximum value is 96 hours (4 days). |
| ![Stress](/images/orbula/dial-stress@2x.png){: width="72"} | Stress |  |
| ![Stress (Graph)](/images/orbula/dial-stress-graph@2x.png){: width="72"} | Stress (Graph) | The graph duration can be changed using the [Graph Duration](#graph-duration) setting. |
| ![Body Battery](/images/orbula/dial-body-battery@2x.png){: width="72"} | Body Battery |  |
| ![Body Battery (Graph)](/images/orbula/dial-body-battery-graph@2x.png){: width="72"} | Body Battery (Graph) | The graph duration can be changed using the [Graph Duration](#graph-duration) setting. |
| ![Run VO2 Max](/images/orbula/dial-run-vo2-max@2x.png){: width="72"} | Run VO2 Max | Maximum value is 60. |
| ![Bike VO2 Max](/images/orbula/dial-bike-vo2-max@2x.png){: width="72"} | Bike VO2 Max | Maximum value is 60. |
| ![Oxygen Saturation](/images/orbula/dial-o2-sat@2x.png){: width="72"} | Oxygen Saturation |  |
| ![Oxygen Saturation (12h Graph)](/images/orbula/dial-o2-sat-graph@2x.png){: width="72"} | Oxygen Saturation (12h Graph) | The graph duration is always 12 hours, as oxygen saturation is recorded infrequently. |
| ![Respiration Rate](/images/orbula/dial-respiration-rate@2x.png){: width="72"} | Respiration Rate | In breaths-per-minute. |
| ![Solar Input](/images/orbula/dial-solar-input@2x.png){: width="72"} | Solar Input | Solar watches only. |
| ![Thermometer](/images/orbula/dial-thermometer@2x.png){: width="72"} | Thermometer | Temperature, as measured by your watch, in degrees **celcius** (metric) or **farenheit** (statute), based on the Temperature Units setting on your watch. |
| ![Thermometer (Graph)](/images/orbula/dial-thermometer-graph@2x.png){: width="72"} | Thermometer (Graph) | Temperature, as measured by your watch, in degrees **celcius** (metric) or **farenheit** (statute), based on the Temperature Units setting on your watch. The graph duration can be changed using the [Graph Duration](#graph-duration) setting. |
| ![Wheelchair Pushes](/images/orbula/dial-wheelchair-pushes@2x.png){: width="72"} | Wheelchair Pushes | In wheelchair mode only. |
| ![Wheelchair Pushes (Daily)](/images/orbula/dial-wheelchair-pushes-daily@2x.png){: width="72"} | Wheelchair Pushes (Daily) | In wheelchair mode only. |
| ![Distance](/images/orbula/dial-distance@2x.png){: width="72"} | Distance | Total distance for the current day, in **km** (metric) or **mi** (statute), based on the Distance Units setting on your watch. |
| ![Alarms](/images/orbula/dial-alarms@2x.png){: width="72"} | Alarms | Number of alarms set on your watch. |

## Icon Row

Choose to show up to 3 additional icons outside of the dials. Defaults are **Battery (%)** and **Bluetooth**. Options are:

| Icon | Name | Notes |
| :-: | :- | :- |
|  | None | Do not show an icon in this position. |
| ![Battery (%)](/images/orbula/icon-battery-percent-green.png){: width="32"}<br>![Battery (%) Low](/images/orbula/icon-battery-percent-yellow.png){: width="32"}<br>![Battery (%) Critical](/images/orbula/icon-battery-percent-red.png){: width="32"}<br>![Battery (%) Charging](/images/orbula/icon-battery-percent-charging.png){: width="32"} | Battery (%) | Current battery level in %. Level shown in <span style="color:#ffaa00">yellow</span> if less than 20%, or <span style="color:red">red</span> if less than 10%. **+** symbol indicates charging. |
| ![Battery (Days)](/images/orbula/icon-battery-days-green.png){: width="32"}<br>![Battery (Days) Low](/images/orbula/icon-battery-days-yellow.png){: width="32"}<br>![Battery (Days) Critical](/images/orbula/icon-battery-days-red.png){: width="32"}<br>![Battery (Days) Charging](/images/orbula/icon-battery-days-charging.png){: width="32"} | Battery (Days) | Current battery level, with estimated remaining battery life in days or hours. |
| ![Battery](/images/orbula/icon-battery-green.png){: width="32"}<br>![Battery Low](/images/orbula/icon-battery-yellow.png){: width="32"}<br>![Battery Critical](/images/orbula/icon-battery-red.png){: width="32"} | Battery | Current battery level icon only. |
| ![Alarms](/images/orbula/icon-alarms.png){: width="32"}<br>![Alarms None](/images/orbula/icon-alarms-disabled.png){: width="32"} | Alarms | Icon will be shown in colour if you have at least one alarm set. |
| ![Bluetooth Connected](/images/orbula/icon-bluetooth.png){: width="32"}<br>![Bluetooth Disconnected](/images/orbula/icon-bluetooth-disabled.png){: width="32"} | Bluetooth | Icon will be shown in colour if your watch has a Bluetooth connection to your phone. |
| ![Notifications](/images/orbula/icon-notifications.png){: width="32"}<br>![Alarms None](/images/orbula/icon-notifications-disabled.png){: width="32"} | Notifications | Icon will be shown in colour if you have at least one unread phone notification. |

## Line Meter

Choose what data the line meter shows. The icon is only shown if the [Line Meter Icon](#line-meter-icon) setting is turned on. Options are:

| Icon | Name | Notes |
| :-: | :- | :- |
|  | None | Hide the meter. |
| None | Move Bar | See [Move Bar](#move-bar) section below. |
| ![Battery](/images/orbula/icon-battery-green.png){: width="32"} | Battery | |
| ![Stress](/images/orbula/icon-stress.png){: width="32"} | Stress | |
| ![Body Battery](/images/orbula/icon-body-battery.png){: width="32"} | Body Battery | |
| ![Oxygen Saturation](/images/orbula/icon-o2-sat.png){: width="32"} | Oxygen Saturation | |
| ![Solar Input](/images/orbula/icon-solar-input.png){: width="32"} | Solar Input | Solar watches only. |

### Move Bar

The Move Bar is a reminder to stay active. It has 5 segments. The first, longer segment, lights up after 1 hour of inactivity. Then, each shorter segments lights up after an additional 15 minutes of inactivity. You can clear the Move Bar by taking a few steps.

| ![Move Bar Level 0](/images/orbula/move-bar-level-0@4x.png){: width="144"} | Active within the last hour. |
| ![Move Bar Level 1](/images/orbula/move-bar-level-1@4x.png){: width="144"} | Inactive for 1 hour. |
| ![Move Bar Level 2](/images/orbula/move-bar-level-2@4x.png){: width="144"} | Inactive for 1 hour 15 mins. |
| ![Move Bar Level 3](/images/orbula/move-bar-level-3@4x.png){: width="144"} | Inactive for 1 hour 30 mins. |
| ![Move Bar Level 4](/images/orbula/move-bar-level-4@4x.png){: width="144"} | Inactive for 1 hour 45 mins. |
| ![Move Bar Level 5](/images/orbula/move-bar-level-5@4x.png){: width="144"} | Inactive for 2 hours or longer. |

## Line Meter Icon

Turn on to show an icon next to the line meter. An icon is never shown for the Move Bar, because its appearance is already distinguishable from other uses of the Line Meter.

## OpenWeather Key

It is currently only possible to enter an OpenWeather key using the Connect IQ mobile app. For more information about how to use Orbula's OpenWeather feature, see the [OpenWeather Integration](#openweather-integration) section below.

## Calories Goal

Goal value for Calories and Active Calories side meters and dials. Choose a value between 200 and 8,000 Calories/kcal. Defaults to 2,000.

## Graph Duration

Time period used by "(Graph)" dials, except for Oxygen Saturation (12h Graph). Choose a value between 1 and 6 hours. Defaults to 1 hour.

## Pressure Units

Units used for the Pressure and Pressure (Graph) dials. Options are:

- **mb/hPa**: millibars/hectopascals (default)
- **inHg**: inches of mercury
- **mmHg**: millimeters of mercury

Note that if your watch has a separate Pressure Units setting, this will **not** be used, due to a technical limitation.

# OpenWeather Integration

[OpenWeather](https://openweathermap.org/) is a popular third-party weather service, offered as an alternative to Garmin's own built-in weather service.

{% capture openweather-sign-up %}
{% include openweather-sign-up.md %}
{% endcapture %}

{{ openweather-sign-up | markdownify }}

Weather-based dials will now show a coloured dot, indicating the status of the OpenWeather data. **It may take up to 5 minutes for the weather data to appear after entering your key.**

![Weather with OpenWeather status](/images/orbula/dial-weather-open-weather@2x.png){: width="72"}
![Weather (Min/Max) with OpenWeather status](/images/orbula/dial-weather-min-max-open-weather@2x.png){: width="72"}
![Humidity with OpenWeather status](/images/orbula/dial-humidity-open-weather@2x.png){: width="72"}

{% capture openweather-status %}
{% include openweather-status.md %}
{% endcapture %}

{{ openweather-status | markdownify }}
