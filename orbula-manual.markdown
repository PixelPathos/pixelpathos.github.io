---
layout: default
title: Orbula Manual
description: Orbula, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /orbula/manual
app_name: Orbula
---
**The Orbula manual is currently a work in progress.**

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
| ![Battery (Days)](/images/orbula/icon-battery.png){: width="32"} | Battery (Days) | Current battery level, with estimated remaining battery life. |
| ![Steps](/images/orbula/icon-steps.png){: width="32"}| Steps | |
| ![Calories](/images/orbula/icon-calories.png){: width="32"} | Calories | Calories burnt for the current day. Calories goal is set manually using the [Calories Goal](#calories-goal) setting. |
| ![Active Calories](/images/orbula/icon-calories.png){: width="32"} | Active Calories | An estimate of active calories burnt for the current day, based on gender, age, height, weight, and total calories. Active calories goal is set manually using the same [Calories Goal](#calories-goal) setting as above. |
| ![Floors Climbed](/images/orbula/icon-floors-climbed.png){: width="32"} | Floors Climbed | Only supported by watches with barometers. |
| ![Active Minutes (Weekly)](/images/orbula/icon-active-minutes.png){: width="32"} | Active Minutes (Weekly) | |
| ![Recovery Time](/images/orbula/icon-recovery-time.png){: width="32"} | Recovery Time | Maximum value is 4 days. |
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
| ![Battery (Days)](/images/orbula/dial-battery-days@2x.png){: width="72"} | Battery (Days) | Current battery level, with estimated remaining battery life. |
| ![Steps](/images/orbula/dial-steps@2x.png){: width="72"} | Steps | |
| ![Steps (Daily)](/images/orbula/dial-steps-daily@2x.png){: width="72"} | Steps (Daily) | Each bar represents the number of steps on that day. The leftmost bar is one week ago, the rightmost <span style="color:white">white</span> bar is today. A <span style="color:red">theme-coloured</span> bar means the goal was achieved that day; otherwise, the bar is <span style="color:#808080">grey</span>, and the thin <span style="color:#808080">grey</span> line shows the goal value. |
| ![Calories](/images/orbula/dial-calories@2x.png){: width="72"} | Calories | Calories goal is set manually using the [Calories Goal](#calories-goal) setting. |
| ![Calories (Daily)](/images/orbula/dial-calories-daily@2x.png){: width="72"} | Calories (Daily) | Calories goal is set manually using the [Calories Goal](#calories-goal) setting, and is used for all days |
| ![Active Calories](/images/orbula/dial-active-calories@2x.png){: width="72"} | Active Calories | An estimate of active calories burnt for the current day, based on gender, age, height, weight, and total calories. Active calories goal is set manually using the same [Calories Goal](#calories-goal) setting as above. |
| ![Floors Climbed](/images/orbula/dial-floors-climbed@2x.png){: width="72"} | Floors Climbed |  |
| ![Floors Climbed Daily](/images/orbula/dial-floors-climbed-daily@2x.png){: width="72"} | Floors Climbed (Daily) |  |
| ![Active Minutes (Weekly)](/images/orbula/dial-active-minutes@2x.png){: width="72"} | Active Minutes (Weekly) |  |
| ![Weather](/images/orbula/dial-weather@2x.png){: width="72"} | Weather | Current forecast temperature and condition. Dial min/max temperatures are for the whole day (Garmin Weather) or the remainder of the day (OpenWeather). |
| ![Weather (Min/Max)](/images/orbula/dial-weather-min-max@2x.png){: width="72"} | Weather (Min/Max) | Current forecast temperature and condition, plus min/max temperatures for the whole day (Garmin Weather) or the remainder of the day (OpenWeather). |
| ![Humidity](/images/orbula/dial-humidity@2x.png){: width="72"} | Humidity |  |
| ![Sunrise/Sunset](/images/orbula/dial-sunrise-sunset@2x.png){: width="72"} | Sunrise/Sunset | Time and type of next "sun event" (sunrise or sunset). Dial represents time between previous and next sun events e.g. how far through daytime you are.  |
| ![Sunrise/Sunset (Today)](/images/orbula/dial-sunrise-sunset-today@2x.png){: width="72"} | Sunrise/Sunset (Today) | Sunrise time (top), sunset time (bottom) and next "sun event" icon (sunrise or sunset). Time of next sun event is shown in <span style="color:white">white</span>. Bar represents the current 24 hours: <span style="color:#808080">grey</span> is night, <span style="color:#ffaa00">yellow</span> is day, and <span style="color:white">white</span> pointer is the current time.|
|  | Altitude |  |
|  | Altitude (Graph) |  |
|  | Pressure |  |
|  | Pressure (Graph) |  |
|  | Notifications |  |
|  | Heart Rate |  |
|  | Heart Rate (Graph) |  |
|  | Heart Rate (Zones) |  |
|  | Weekly Run Distance |  |
|  | Weekly Bike Distance |  |
|  | Recovery Time |  |
|  | Stress |  |
|  | Stress (Graph) |  |
|  | Body Battery |  |
|  | Body Battery (Graph) |  |
|  | Run VO2 Max |  |
|  | Bike VO2 Max |  |
|  | Oxygen Saturation |  |
|  | Oxygen Saturation (12h Graph) |  |
|  | Respiration Rate |  |
|  | Solar Input |  |
|  | Thermometer |  |
|  | Thermometer (Graph) |  |
|  | Wheelchair Pushes |  |
|  | Wheelchair Pushes (Daily) |  |
|  | Distance |  |
|  | Alarms |  |