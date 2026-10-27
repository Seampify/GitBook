# Calling through WhatsApp Cloud API

In 15th July 2025, Meta have released the Cloud API Calling solution where brand can now initiate and receive calls with users on WhatsApp using voice-over-internet protocol (VoIP).

## **Get Started with Cloud API Calling**

## Step 1: Prerequisites

Before you get started with the Calling API, ensure that:

1. Your business number is in use with Cloud API (not the WhatsApp Business app)
2. The business phone number should be in the Messaging Tier of at-least 2,000 (2K) messages. [More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)
3. Enable Calling features on your business phone number:

{% stepper %}
{% step %}
Go to Settings > Channels or [https://waba.seampify.com/settings/channels](https://waba.seampify.com/settings/channels). Then, click on the **General Settings** button of the Cloud API channel

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Click on the **Calls** tab and enable the Allow voice calls function.

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Calling is not default enabled on a business phone number
{% endhint %}

## Step 2: Configure optional calling features

The WhatsApp Business Calling API offers a number of features that affect when and how calling features appear to users on your WhatsApp profile

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-06 at 2.43.27 PM.png" alt=""><figcaption></figcaption></figure>

### Allow voice calls

This is the master function to enable or disable voice calls in your WhatsApp Account (WABA).

### Allow people to request a callback for missed calls

When this is enabled, customer is able to request for a callback if you have missed the calls.

{% hint style="warning" %}
The [Availaible call hours](./#available-call-hours) need to be set up for thos to work.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

### Display call buttons

When Calling API features are enabled for a business number, you can still choose whether to show the call button icon or not by using the Display call buttons function.

{% hint style="info" %}
Note: Disabling call button icon visibility does not disable a WhatsApp user’s ability to make calls to your business.
{% endhint %}

The behavior for supported options is as follows:

**DEFAULT**

The Call button icon will be displayed in the chat menu bar and the business info page, allowing for incoming calls to the business by WhatsApp users.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

**DISABLE ALL**

The call button icon is hidden in the chat menu bar and the business info page, and all other entry points external to the chat are also disabled. Consumers cannot make unsolicited calls to the business.

Your business can still send interactive messages or template messages with a Calling API CTA button.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### **Available call hours**

With the Available call hours setting, you can specify the timezone, business operating hours, and holiday schedules that will be enforced for all user-initiated calls.

Configuring this setting restricts calls only to available weekly hours you configure. User-initiated calls are unavailable outside of the weekly hours and holiday schedules you set.

The WhatsApp client app will show users an option to chat with the business, or request a callback, if Allow people to request a callback for missed calls is ENABLED. The user will also be shown the next available calling slot on the option screen.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

### Callback permissions

Calling a WhatsApp user requires explicit permission from the user. One way to obtain calling permissions is to request permission when a WhatsApp user calls your business.

You can configure the call permission UI to automatically show in the WhatsApp user’s client app when they call your business number. The user may change their permission selection at any time.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

## Step 3: Make and receive calls

Cloud API Calling offers two call initiation paths:

[**User-initiated calls:**](user-initiated-calls.md)\
Calls that are made from a WhatsApp user to your business\
\
[**Business-initiated calls:**](business-initiated-calls.md)\
Calls that are made from your business to a WhatsApp user<br>

## Availability

**User-initiated Calling (UIC)**\
UIC is available in every location Cloud API is available

**Business-initiated Calling (BIC)**\
BIC is currently available in every location Cloud API is available, except the following countries:

USA\
Canada\
Turkey\
Egypt\
Vietnam\
Nigeria<br>

{% hint style="warning" %}
Note: The business phone number’s country code must be in this supported list. The consumer phone number can be from any country where Cloud API is available.
{% endhint %}
