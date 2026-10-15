# Business-initiated Calls

The Calling API supports making calls to WhatsApp users from your business.

The user dictates when calls can be received by [granting call permissions to the business phone number](business-initiated-calls.md#obtain-user-call-permissions).



## Obtain User Call Permissions <a href="#part-1--obtain-permission-to-call-the-whatsapp-user" id="part-1--obtain-permission-to-call-the-whatsapp-user"></a>

If you want to place a call to a WhatsApp user, your business must receive user permission first. When a WhatsApp user grants call permissions, they are always temporary **for 7 calendar days (168 hours).**

You can obtain calling permission from a WhatsApp user in any of the following ways:

1. [**Request a call permission request to the user**](business-initiated-calls.md#request-a-call-permission-request-to-the-user)&#x20;
2. [**Callback permission is provided by the WhatsApp user** ](business-initiated-calls.md#callback-permission-is-provided-by-the-whatsapp-user)
3. When a WhatsApp user calls you, regardless of if you accept the call or not

&#x20;

### **Request a call permission request to the user**&#x20;

A call permission request message can be sent to users in one of the following ways:

* [Create and send a template message](business-initiated-calls.md#create-and-send-a-template-message)
* [Send a free form message](business-initiated-calls.md#send-a-free-form-message)

#### **1. Create and send a template message**

Firstly, setup a call permission template message by going to [Manage Template](../../seampifys-modules/settings/more-settings/channels/manage-templates/#create-a-template-messages) and select Call Permission Request message type. Click Sumit For Approval once done.

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Call Permission Request template message is availiable under Marketing and Utility category.
{% endhint %}

Once the template message is approved, you may use it to sent to your contact. Go to Chat and look for the contact in the WhatsApp Cloud API Channel, you will see a **Request Call Permission** button on top right.&#x20;

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

Click on the Request Call Permission to choose the templates message. Setup the placeholder (if any) then, select **Confirm** to sent to the contact.

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**Note:** Call permission request template messages are subject to [messaging charges](../conversation-through-whatsapp-cloud-api/whatsapp-conversation-based-pricing/)
{% endhint %}

This is what your customer will see and allow the permission to you.

<figure><img src="../../.gitbook/assets/Allow call.jpg" alt=""><figcaption></figcaption></figure>



#### **2. Send a free form message**

When you are within a customer service window with a WhatsApp user, you can send a free form message with a call permission request.

\
Firstly, go to the Chat page and open the conversation with the Contact that you wish to request for permission. Click on the <img src="../../.gitbook/assets/image (49).png" alt="" data-size="line"> button at the bottom and slect Send Buttons/Flows/Options/Products Message button<br>

<figure><img src="../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

It will opens the Interactive Message settings. Click on the **Call Permission Request** message type and fill in your message. Then, select **Send**.

<figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

This is what your customer will see and allow the permission to you.

<figure><img src="../../.gitbook/assets/Allow call.jpg" alt=""><figcaption></figcaption></figure>



### **Callback permission is provided by the WhatsApp user**&#x20;

The WhatsApp user automatically provides temporary call permissions by placing a call to the business. The [callback setting must be enabled](./#callback-permissions) on the business phone number.<br>

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>



## Performing a Business-initiated Calls <a href="#limits-per-business-whatsapp-user-pair" id="limits-per-business-whatsapp-user-pair"></a>

The WhatsApp user may approve, decline, or simply not respond to a call permission request. Once you have user permission,  you will see the call button and the permission duration on the top right and you may click to perform a Business-Initiated Call with the Contact.

<figure><img src="../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Business-initiated calls is subject to [Calling API Pricing.](calling-api-pricing.md)
{% endhint %}



## Limits (Per business + WhatsApp user pair) <a href="#limits-per-business-whatsapp-user-pair" id="limits-per-business-whatsapp-user-pair"></a>

* Temporary permissions are **granted for 7 calendar days (168 hours),** if the user call your business first.
  * Calculated as the number of seconds in a day multiplied by 7, from time of user’s approval.
* Your business can make up to **10 calls every 24 hours/per user**
* Your business can make only **5 connected calls every 24 hours/per user**
* These limits are on the **business phone number**

These limits are in place to protect WhatsApp users from unwanted calls

## User Preference Options

When your business sends a call request on WhatsApp, the customer is presented with three distinct options to manage their privacy: **Allow, Allow temporarily, and Not at this time**. These preferences determine how long your business has permission to initiate voice calls to that specific contact.

* **Allow:** This grants your business ongoing permission to initiate calls to the customer. The permission remains active until the user manually changes their preference or blocks the business.
* **Allow temporarily:** This grants permission for exactly 7 calendar days (168 hours). After this period expires, your business must send a new permission request to initiate another call.
* **Not at this time:** This declines the current request. Your business will not be able to initiate a call, and you should wait for a reasonable period or a new customer interaction before requesting permission again to avoid being flagged for spam.



## Call Permission Request Basics <a href="#call-permission-request-basics" id="call-permission-request-basics"></a>

**The WhatsApp user is in control.** Even if the user provides calling permission, they can revoke that granted permission request at any time. Conversely, if the user declines a permission request, they can still grant calling permission, up until the permission request expires.



**A call permission request expires** when any of the following occurs:

* The WhatsApp user interacts with a subsequent new call permission request from the business

<figure><img src="../../.gitbook/assets/image (16).png" alt="" width="375"><figcaption></figcaption></figure>

* 7 days after the permission was accepted or declined by the consumer

<figure><img src="../../.gitbook/assets/image (13).png" alt="" width="180"><figcaption></figcaption></figure>

* 7 days after the permission was delivered if the consumer does not respond to the request

<figure><img src="../../.gitbook/assets/image (14).png" alt="" width="179"><figcaption></figcaption></figure>



## Call Permission Request Limits

To ensure an optimal user experience around business initiated calling, the following limits are enforced:

1. **When sending a calling permission request message**
   * Maximum of 1 permission request in 24h
   * Maximum 2 permission requests within 7 days.
     * _These limits reset when any connected call (business-initiated/user-initiated) is made between the business and WhatsApp user._
     * _These limits apply toward permissions requests sent either as free form or template messages._
2.  **When business-initiated calls go unanswered or are rejected**

    * 2 consecutive unanswered calls result in system message to reconsider an approved permission

    <figure><img src="../../.gitbook/assets/2 consecutive unasnwered.jpg" alt=""><figcaption></figcaption></figure>

    * 4 consecutive unanswered calls result in an approved permission being automatically revoked. The user may again update this if they so choose.

    <figure><img src="../../.gitbook/assets/4 consecutive unasnwered.jpg" alt=""><figcaption></figcaption></figure>



## Frequently Asked Question about Business-initiated Calls

<details>

<summary>Am I eligible for WhatsApp calling?</summary>

Before you get started with the Calling API, ensure that:

1. Your business number is in use with Cloud API (not the WhatsApp Business app)
2. The business phone number should be in the Messaging Tier of at-least 2,000 (2K) messages. [More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)
3. [Enable Calling features on your business phone number](./#step-1-prerequisites)

</details>

<details>

<summary>What are the countries supported for calling?</summary>

**User-initiated Calling (UIC)**\
UIC is available in every location Cloud API is available

**Business-initiated Calling (BIC)**\
BIC is currently available in every location Cloud API is available, except the following countries:

USA\
Canada\
Turkey\
Egypt\
Vietnam\
Nigeria

{% hint style="warning" %}
Note: The business phone number’s country code must be in this supported list. The consumer phone number can be from any country where Cloud API is available.
{% endhint %}

</details>

<details>

<summary>Does the WABA need to have an attached credit line for using Calling APIs?</summary>

Yes, you need a credit line attached to your WABA in order to use the Calling API. [Refer to Calling API Pricing for the rate card.](calling-api-pricing.md#volume-based-pricing--vbp--rate-card)

</details>

<details>

<summary>What WhatsApp versions and client platforms support the business initiated calling feature?</summary>

WhatsApp Client versions 2.24.14.x and onwards support the call permission requests and business initiated calling feature.

Both WhatsApp Android and iOS platforms support the feature.

</details>

<details>

<summary>Does the permission expire after five connected calls have been made?</summary>

5 connected calls in 24 hours is simply a time window based running limit. Reaching that limit does not close the permission, permission remains open until the full 7 days. The 6th call can happen 24hrs after the 1st call.

We can simply think of this as a rate limit for business initiated calls. A maximum of 35 calls can happen over 7 days.

</details>

<details>

<summary>Is there a way to reset the call permission request limits?</summary>

A connected call will reset the [call permission request limits](business-initiated-calls.md#call-permission-request-limits)

</details>

<details>

<summary>What happens if the WhatsApp user has set up <a href="https://faq.whatsapp.com/1238612517047244/?cms_platform=android&#x26;fbclid=IwZXh0bgNhZW0CMTEAYnJpZBExQTBLZ01YQkJxVTNZSTRiQgEevQ9SUDauHlsOFgILu6BxDC2AeMO--nIma1RftSUnLXCs9Pk7RuLyt3T_zoU_aem_owpp5XKRKRdFeuaOYRrrCg">Silence Unknown Callers</a> settings?</summary>

Business initiated calls bypass ‘Silence Unknown Callers’ settings since the call can only happen after explicit permission provided by the user.

</details>

<details>

<summary>Can we place a call with an ongoing number?</summary>

No, you are not able to place a call when it is already ongoing with the receiver.

</details>
