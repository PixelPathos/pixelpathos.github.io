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
- The number of satellite dials from 3 to 6;
- The position of the time dial;
- The theme, background and icon colours;
- The time format (12/24 hour, and leading zero);
- The font and colour of the hours, separator and minutes, and the type of separator;
- The data shown on the side meters, dials and line meter;
- The icons;
- The brightness of the always-on display (AMOLED only).

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
| Colourful Icons On | Colourful Icons Off |

If turned on, complication icons are shown in distinct colours e.g. blue for body battery, purple for floors climbed. If turned off, all icons are shown in the [theme colour](#theme-colour).
