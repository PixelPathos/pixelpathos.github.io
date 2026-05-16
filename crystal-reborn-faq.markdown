---
layout: default
title: Crystal Reborn FAQ
description: Crystal Reborn, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /crystal-reborn/faq
---
![Crystal Reborn hero image](/images/crystal-reborn/hero-image.png)

## General

### What if my question isn't answered here?
Please contact me via the ```App Support``` link on the appropriate Crystal Reborn store page ([Garmin Pay]({{ site.crystal_reborn_store_url }}) or [KiezelPay]({{ site.crystal_reborn_kpay_store_url }})) and I'll be in touch.

### Crystal Reborn versions

{% capture versions %}
{% include gpay-kpay-versions.md
    app_name="Crystal Reborn"
    gpay_store_url=site.crystal_reborn_store_url
    kpay_store_url=site.crystal_reborn_kpay_store_url
    kpay_trial_hours=site.crystal_reborn_kpay_trial_hours
%}
{% endcapture %}

{{ versions | markdownify }}

### Crystal Reborn won't install. Help!
Firstly, ensure your watch is [running the latest firmware](https://support.garmin.com/en-GB/?faq=ZKn5UHHyEF9J3MPROKwRj8). This should happen automatically, but there may be a short delay between the firmware becoming available, and it installing on your watch.

If that hasn't helped, try:
- Turning Bluetooth off and on again;
- Restarting your watch and your phone;
- Re-pairing your watch with your phone;
- Re-installing the Connect IQ app.

## Features

### How do I customise Crystal Reborn?
The easiest way is via the watch face settings **on the watch itself**. This varies slightly by model, but is something like ```[Main Menu] > Watch Face > [Edit] > Settings```. This will be the same as for other built-in and third-party watch faces.

Alternatively, you can use the **Connect IQ phone app**. From the main app screen: ```My Device > My Watch Faces > Crystal Reborn > Settings```.

For more information about what you can customise, see the [Crystal Reborn manual](/crystal-reborn/manual).

### How do I change between 12-hour and 24-hour format?
Change the **time format setting** via the general settings menu on your watch, and Crystal Reborn will pick up the change - there isn't a separate Crystal Reborn setting.