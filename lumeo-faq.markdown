---
layout: default
title: Lumeo FAQ
description: Lumeo, a Garmin Connect IQ watch face by Pixel Pathos
permalink: /lumeo/faq
---
![Lumeo hero image](/images/lumeo-hero-image.png)

## General

### Why are there two versions of Lumeo?
The original version of [Lumeo]({{ site.lumeo_store_url }}) only accepts payments via **Garmin Pay**.

Because Garmin Pay only supports a limited number of banks, by popular request, a separate version, [Lumeo (KiezelPay)]({{ site.lumeo_kpay_store_url }}), accepts payments via **KiezelPay**. You can pay using PayPal (no additional fee, recommended), or direct credit card payments ($0.30 fee).

### Which version of Lumeo is better?
Both Garmin Pay and KiezelPay versions of Lumeo will receive exactly the same feature updates, bug fixes and support, except where a fix is related to the payment system itself.

### Why is the KiezelPay version more expensive?
This is because KiezelPay charges developers nearly double the fee compared to Garmin Pay. The KiezelPay version is priced so that Pixel Pathos receives approximately the same payment as the Garmin Pay version.

### Is the payment one-off, or a monthly subscription?
It's one-off. There are no ongoing charges.

### What if my question isn't answered here?
Please contact me via the ```Contact Developer``` link on the appropriate Lumeo store page ([Garmin Pay]({{ site.lumeo_store_url }}) or [KiezelPay]({{ site.lumeo_kpay_store_url }})) and I'll be in touch.

### Where can I download Lumeo?
Find Lumeo on Garmin's Connect IQ Store: [Garmin Pay]({{ site.lumeo_store_url }}) or [KiezelPay]({{ site.lumeo_kpay_store_url }})).

### Lumeo won't install. Help!
Firstly, ensure your watch is [running the latest firmware](https://support.garmin.com/en-GB/?faq=ZKn5UHHyEF9J3MPROKwRj8). This should happen automatically, but there may be a short delay between the firmware becoming available, and it installing on your watch.

If that hasn't helped, try:
- Turning Bluetooth off and on again;
- Restarting your watch and your phone;
- Re-pairing your watch with your phone;
- Re-installing the Connect IQ app.

## Garmin Pay version

### Can I trial Lumeo before paying?
Garmin Pay requires that you pay up front, but you then have 48 hours to try Lumeo. If you are not happy, you can [request a full refund]({{ site.garmin_refund_url }}) within that period.

### Garmin Pay doesn't work with my payment card, or in my country. Is there another way I can pay for Lumeo?
The separate [KiezelPay version of Lumeo]({{ site.lumeo_kpay_store_url }}) (also see below) accepts payments via PayPal and credit card.

### I'm not happy with Lumeo. How do I get a refund?
I'm sorry to hear that. Garmin will allow you to [request a full refund]({{ site.garmin_refund_url }}) within the first 48 hours after purchase.

If you're considering asking for a refund, I'd appreciate it if you could contact me via [Lumeo's store page]({{ site.lumeo_store_url }}) to let me know what I can improve.

## KiezelPay version

### How does KiezelPay work?
Download and install Lumeo as normal. You will then have {{ site.lumeo_kpay_trial_hours }} hours to try Lumeo, completely free. After this period, Lumeo will show a 6-digit code. You will then need to go to www.kzl.io/code and enter the code. You will then be able to make a payment, and Lumeo will unlock.

### Why does Lumeo need to run in the background, and access the internet?
This is to allow the KiezelPay integration to access the KiezelPay servers only, to check payment status.

### Can I get a refund?
You can get a refund within 30 days of purchasing the KiezelPay version of Lumeo by following the instructions [here](https://kiezelpay.com/faq/faq-refund).

If you're considering asking for a refund, I'd appreciate it if you could contact me via [Lumeo (KiezelPay)'s store page]({{ site.lumeo_kpay_store_url }}) to let me know what I can improve.

## Features

### How do I customise Lumeo?
On most watches, you can customise Lumeo via the watch face settings **on the watch itself**. Google ```watch face settings <my watch model>``` for the relevant page of the online owner's manual.

If your model does not support on-device settings, then you will need to use the **Connect IQ phone app** to customise Lumeo. From the main app screen: ```My Device > My Watch Faces > Lumeo > Settings```.

### What can I customise on Lumeo?
Almost everything: the layout, the colour, which complications are shown, the styles of the dials and meters, which indicators are shown, how long the graph history is, and so on.

### How do custom themes work?
A Lumeo custom theme consists of 3 colours:
- A "bright" colour, that's used for the dots on the meters, as well as the top of the time and meter gradients;
- A "main" colour, that's used for all the icons and coloured text, as well as the middle of the gradients;
- A "dark" colour, that's used for the bottom of the gradients.

The easiest way to edit the theme is on the watch itself:
- On AMOLED watches, the custom theme is the last theme in the list. The custom theme preview will show a "cog" icon. Tap that to open the theme editor.
- On MIP watches, ensure the custom theme is selected. Then, there is a separate ```Edit Custom Theme``` top-level menu item which will open the theme editor.

The theme editor shows the 3 theme colours at the bottom (bright/main/dark in that order). It shows which one is currently being edited, and a preview of how the gradient will look.

Select the colour you wish to edit, then edit it using the colour wheel and square (AMOLED) or the colour picker (MIP).

The custom theme is stored as a single string of 3 ```#RRGGBB``` hex codes (bright/main/dark), as shown in the theme editor. These codes can be manually entered into the Custom Theme setting when editing Lumeo's settings in the Connect IQ app on your phone. This means that themes can be shared online.

![Lumeo's Colour Picker](/images/lumeo-colour-picker.png)

### What are the grey dots/coloured dashes?
This is Lumeo's "stealth" version of the Garmin Move Bar. You can turn it off in settings.

The Move Bar has 5 segments. The first, longer segment, lights up after 1 hour of inactivity. Then, each shorter segments lights up after an additional 15 minutes of inactivity. You can clear the Move Bar by taking a few steps.

![Lumeo's Move Bar](/images/lumeo-move-bar.png){: width="442"}

### Why can't I change between 12-hour and 24-hour format?
You can change this via a **separate time format setting** on your watch - it's not a Lumeo setting, but Lumeo will respect it. Google ```change time format <my watch model>``` for the relevant page of the online owner's manual.

### Why does a symbol appear in grey on the watch face?
It's most likely because Lumeo can't determine a value for now. For example, if you take the watch off, it can't measure heart rate, so the heart symbol will appear in grey.

If your watch is a long distance from your phone, it will lose Bluetooth connection, and the Bluetooth symbol will appear in grey.

It may also be that your device does not support that particular complication. For example, Approach® S50 and vívoactive® 5 devices don't support Floors Climbed, so that symbol will appear in grey.

### What is OpenWeather/Advanced Weather?
Find out more about Lumeo's weather features [here](/lumeo/weather).