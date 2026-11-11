# User-initiated Calls

The Calling API supports receiving calls made by WhatsApp users to your business for free.

Your business dictates when calls can be received by configuring business calling hours and holiday unavailability from the calling feature settings.

{% hint style="success" %}
[Before you get started with user-initiated calling, ensure that you have enable the Calling API features on your business phone number.](./#step-1-prerequisites)
{% endhint %}

Once a call is established, there is about 30 to 60 seconds for the business to accept the phone call. If the business does not respond, the call is terminated on the WhatsApp user side with a "Not Answered" notification.



## Promoting your WhatsApp Call

After you adopt Cloud API Calling features, you can raise awareness with your customers in two core ways:

* [Send them a message with a WhatsApp call button](user-initiated-calls.md#send-interactive-message-with-a-whatsapp-call-button)
* [Embed a calling deep link into your brand surfaces (website, application, etc)](user-initiated-calls.md#calling-deep-links)



### Send message with a WhatsApp Call Button <a href="#send-interactive-message-with-a-whatsapp-call-button" id="send-interactive-message-with-a-whatsapp-call-button"></a>

There are 2 types of message where you can allow your customer to perform a call to your number:

* Interactive message - a free form interactive message with a WhatsApp call button during a [customer service window](../conversation-through-whatsapp-cloud-api/understanding-24-hour-customer-service-window.md)
* Template message - marketing or utility template message with a WhatsApp call button outside the [customer service window](../conversation-through-whatsapp-cloud-api/understanding-24-hour-customer-service-window.md)&#x20;

When a WhatsApp user clicks the call button, it initiates a WhatsApp call to the business number that sent the message.

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>



### Creating a calling deep links <a href="#calling-deep-links" id="calling-deep-links"></a>

Calling deep links are hyperlinks that route WhatsApp users to call your business. The process to create a calling deep link is the same as a chat deep link.

**Create your own calling deep link**\
Use https://wa.me/call/ where the is a full phone number in international format. Omit any zeroes, brackets, or dashes when adding the phone number in international format.<br>

**Examples:**\
Use: https://wa.me/call/1XXXXXXXXXX\
Don't use: https://wa.me/call/+001-(XXX)XXXXXXX

{% hint style="danger" %}
Note that deep links are not supported on WhatsApp desktop clients.
{% endhint %}

#### Embed calling deep links <a href="#embed-calling-deep-links" id="embed-calling-deep-links"></a>

You can use calling deep links to advertise WhatsApp calling for your business

Use these links anywhere where calling can be useful, like your website, primary application, or even as a QR code to be shared.

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

#### Send calling deep links <a href="#send-calling-deep-links" id="send-calling-deep-links"></a>

You can also send messages to WhatsApp users with a calling deep link.

Since deep links can be made per business phone number, you can use calling deep links to prompt WhatsApp users to contact a different phone number with voice enabled.

The `wa.me/call/<BUSINESS_PHONE_NUMBER>` format is easy to copy, paste, and send, and does not require you to make a template in Business Manager.

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>



## Frequently Asked Question about User-initiated Calls

<details>

<summary>Am I eligible for WhatsApp calling?</summary>

Before you get started with the Calling API, ensure that:

1. Your business number is in use with Cloud API (not the WhatsApp Business app)
2. The business phone number should be in the Messaging Tier of at-least 2,000 (2K) messages. [More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)
3. [Enable Calling features on your business phone number](./#step-1-prerequisites)

</details>

<details>

<summary>What is the max number of concurrent calls that a single Cloud API account phone number can receive?</summary>

Max concurrent calls is 1000

When the rate limit exceeds, the caller (viz. WhatsApp user) will get a generic message saying call cannot be placed. Meta anticipate to increase this limit and hence chances of this happening are low.

Note that the rate limits for messaging API and template creation/update API are separate and unrelated to calling limits.

</details>

<details>

<summary>What is the maximum call duration supported</summary>

There is no call duration limit

</details>

<details>

<summary>Can I send/receive text/media messages while a call is in progress?</summary>

Yes. The regular send-message API can be used while a call is in progress.

</details>

<details>

<summary>Does the WABA need to be a verified business for calling</summary>

No. [Business verification](../../starting-with-seampify/meta-business-verification.md) is not a requirement for calling, nor is it required for messaging. But, The business phone number should be in the Messaging Tier of at-least 2,000 (2K) messages to be eligible for WhatsApp calling. [More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)

</details>

<details>

<summary>How does usage of Calling APIs affect my rate limits?</summary>

Calling API usage does not count towards messaging rate limits at the moment. The only limit enforced for calling right now is the 1000 concurrent calls limit, but this may change in near future.

</details>

<details>

<summary>When is the call icon in the chat title bar visible on WhatsApp Consumer apps?</summary>

It is visible when **all the following conditions are met:**

* The business phone number has the calling status set to `ENABLED` in the [call settings API](./#step-2-configure-optional-calling-features).
* Call setting display call button is set to `ENABLED` in the [call settings API](./#step-2-configure-optional-calling-features).
  * The call icon visibility feature is supported in WhatsApp mobile versions 2.24.10.8 and above on Android and iOS
* Consumer’s WhatsApp version 2.23.14 or above. We expect all consumers to be on this version or above

</details>

<details>

<summary>Can we limit calling access to specific or individual WA users instead of all WA users? Example: a lead that’s qualified or a customer who is in premium tier</summary>

No, Meta do not have a way to control visibility or access of calling on an individual WhatsApp user basis. However you can use [Call Settings API](./#step-2-configure-optional-calling-features) to set `call_icon_visibility` to `DISABLE_ALL` which will hide call icons to all WA users. For qualified WA users, you can send a message with the call CTA button so only they can call you by tapping on the button in the message

Providing this type of feature would require Meta to store configuration per WhatsApp user which has higher privacy risk. It will also incur higher operational overhead for you to maintain large lists of allowlisted WA users on an ongoing basis

</details>

<details>

<summary>When the call icon is hidden using Call Settings API, is it still possible for consumers to call the business?</summary>

Yes.

A user can still call the business from other entry points which are unaffected by the [Call Settings API](./#step-2-configure-optional-calling-features) such as:

* Save the business number as a contact and use new call
* Call logs from Calls tab > Recent
* Call CTA in messages sent from the business
* Call bubble in the chat window that appears following any call between user and business

Hence the recommendation is to treat `DISABLE_ALL` only as a broad first level filter and ensure your automation in Seampify do any additional filtering based on your own business logic.

</details>

<details>

<summary>What is the min version of WhatsApp mobile apps that support the voice call button?</summary>

* Min app version for iOS is 24.1
* Min app version for Android is 2.

</details>

<details>

<summary>Is calling supported for end users from WhatsApp Web or WhatsApp Desktop apps?</summary>

No. WhatsApp Web does not support consumer-v-consumer or business calls. Desktop apps support only consumer-v-consumer calls at this point

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
