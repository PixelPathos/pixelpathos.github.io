{% comment %}
Expected parameters:
- page.app_name
{% endcomment %}

| Dot Colour | Meaning |
| --- | --- |
| <span style="color:#666666">Grey</span> | No internet connection, or other request error. Ensure your watch is paired with your phone, and that your phone has internet access. |
| <span style="color:#ffaa00">Yellow</span> | Your location can't be determined, so {{ page.app_name }} can't request the weather for your location. {{ page.app_name }} initially requires a location from Garmin Weather, so ensure your watch is paired with your phone, and that your phone has internet access. {{ page.app_name }} will store your current location in case a live location is no longer available. |
| <span style="color:red">Red</span> | Invalid API Key. Check that you have entered a valid OpenWeather key. |
| <span style="color:#ff5500">Orange</span> | Other HTTP error. |
| <span style="color:#00aaff">Blue</span> | A request to OpenWeather has been queued, and will be made within the next 5 minutes. **If you have just set up OpenWeather, no data will be visible until the initial request has completed.** |
| <span style="color:white">White</span> | Successfully sent a request to OpenWeather; now awaiting the reply. |
| <span style="color:#00ff00">Green</span> | Up-to-date weather information successfully received. This indication will automatically disappear after 1 minute. |
