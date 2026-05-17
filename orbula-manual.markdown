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
- The [number of satellite dials](#layout) from 3 to 6;
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

{{ settings-menu-manual-page    s | markdownify }}

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

Control the appearance of the separator.

### Show Hours Leading Zero

If the hour number would be a single digit, add a zero before that digit. Default is off.

### Show Seconds

Default is on. Note that AMOLED devices will always hide the seconds in always on mode, regardless of this setting.



