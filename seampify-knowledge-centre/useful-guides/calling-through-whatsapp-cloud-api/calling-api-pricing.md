# Calling API Pricing

Placing business-initiated calls is charged based on:

* The duration of the call (calculated in six-second increments, rounding up)
* The country code of the phone number associated with the user being called.

A valid payment method is required to place calls.

**Note:** Call permission request template messages are subject to [messaging charges](../conversation-through-whatsapp-cloud-api-1/whatsapp-conversation-based-pricing/)

## Volume-Based Pricing (VBP) Rate card <a href="#volume-based-pricing--vbp--rate-card" id="volume-based-pricing--vbp--rate-card"></a>

These rate cards represent the current VBP rates for the WhatsApp Business Calling API:

{% hint style="info" %}
Cost per minute in USD on the WhatsApp Business Platform, effective April 1, 2026.
{% endhint %}

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Business-initiated call minutes (per month)</strong></td><td valign="top"><strong>Meta rate (MYR) for Malaysia recipient numbers +60</strong></td></tr><tr><td valign="top">1 -50,000</td><td valign="top">0.0435</td></tr><tr><td valign="top">50,001 - 250,000</td><td valign="top">0.0379</td></tr><tr><td valign="top">250,001 - 1,000,000</td><td valign="top">0.0286</td></tr><tr><td valign="top">1,000,001 -2,500,000</td><td valign="top">0.0278</td></tr><tr><td valign="top">2,500,001 - 5,000,000</td><td valign="top">0.0238</td></tr><tr><td valign="top">5,000,001 and above</td><td valign="top">0.0213</td></tr></tbody></table>

{% hint style="warning" %}
[Click to view the Meta rate card.](https://developers.facebook.com/documentation/business-messaging/whatsapp/calling/pricing)
{% endhint %}

### Example Charges

Meta charges your call **every 6 seconds**, not per second or per full minute.\
Each 6-second block is called a **pulse**.

Example:

* If your call lasts **4 seconds**, you are charged for **6 seconds**
* If your call lasts **7 seconds**, you are charged for **12 seconds**
* If your call lasts **20 seconds**, you are charged for **24 seconds**

So the system always **rounds up** to the next 6-second block.

Here's an example calculation for the Business-initiated Calls to a Malaysia country code number:

Rate card: MYR 0.0435 per minute

Actual Call Length: 22 seconds

Billed Duration: 24 seconds rounded up (4 pulses)

Cost: 0.0435 × 4 = **MYR 0.174**

## How calling changes the 24 hour customer service window <a href="#how-calling-changes-the-24-hour-customer-service-window" id="how-calling-changes-the-24-hour-customer-service-window"></a>

{% hint style="info" %}
Available since October 1, 2024
{% endhint %}

Currently, when a WhatsApp user messages you, a [24-hour timer called a customer service window](../conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md) begins, or refreshes.

When you are within the window, your business is allowed to send any type of message to the WhatsApp user, which is otherwise not allowed.

With the introduction of the Calling API, the customer service window now also starts or refreshes for calls:

* When a WhatsApp user calls you, regardless of if you accept the call or not
* When a WhatsApp user accepts your call.
