{% comment %}
Expected parameters:
- app_name
- gpay_store_url
- kpay_store_url
- kpay_trial_hours
{% endcomment %}

There are two versions of {{ include.app_name }} available in the Connect IQ store. There is no difference in features between the two versions.

| | Garmin Pay | KiezelPay |
| ----- | ----- | ----- |
| **Description** | First-party payments handled by Garmin. **RECOMMENDED**, if supported by your region and bank. | Third-party payments handled by KiezelPay. |
| **Store URL** | [Garmin Pay store page]({{ include.gpay_store_url }}). | [KiezelPay store page]({{ include.kpay_store_url }}). |
| **Supported regions** | Please see [this list of regions]({{ site.garmin_regions_url }}) supported by Garmin for first-party purchases. | All regions supported by PayPal, or your chosen payment method. |
| **Payment methods** | By **card** added to Garmin Pay, from a smaller range of banks. | **PayPal** (free). Also by **card**, from a wider range of banks ($0.30 fee). |
| **Price** | **Cheaper** (exact price varies by region). | **More expensive**, because KiezelPay charges developers nearly double the fee compared to Garmin. |
| **Purchase process** | Payment is required before download. Garmin will send an e-mail once your payment has been processed. {{ include.app_name }} will then download and install automatically the next time your watch syncs. | Download is free. You will then have a {{ include.kpay_trial_hours }}-hour trial. When the trial ends, you will be shown a 6-digit code and URL you can use to make the purchase via the KiezelPay site. Within 5 minutes of completing the purchase, {{ include.app_name }} will unlock. |
| **Purchase type** | One-off (not subscription). Purchase is forever, and tied to your Garmin account. | One-off (not subscription). Purchase is forever, and tied to your Garmin account. |
| **Refunds** | Please [contact Garmin directly]({{ site.garmin_refund_url }}) to request a refund within 48 hours of purchase. | Please [follow these instructions]({{ site.kpay_refund_url }}) to request a refund from KiezelPay within 30 days of purchase. |

If you're considering a refund, please contact me first via the ```App Support``` link on the appropriate store page, as I would like to try and make things right.
