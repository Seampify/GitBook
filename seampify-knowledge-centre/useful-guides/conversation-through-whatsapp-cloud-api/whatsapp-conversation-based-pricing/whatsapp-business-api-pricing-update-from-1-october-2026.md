# WhatsApp Business API Pricing Update From 1 October 2026

Meta is introducing an important update to the WhatsApp Business Platform pricing model from **1 October 2026**.

The biggest change is that **Service messages — normal replies sent through the WhatsApp Business API within the 24-hour customer service window — will move to a per-message charging model.**

However, Meta has also announced a new monthly free allowance:

#### Every business phone number will receive 1,000 free Service messages each month.

Meta will only begin charging for Service messages from the **1,001st Service message onwards** for each business phone number during that month.

The 1,000 free Service messages reset every month and **unused messages do not roll over to the following month**.

For businesses using WhatsApp for customer service, sales, chatbot automation and AI, this means the impact of the new pricing model will depend largely on the volume and efficiency of their customer conversations.

***

## What Is Changing From 1 October 2026?

Today, when a customer sends your business a WhatsApp message, a **24-hour customer service window** opens.

During this window, businesses can send normal non-template replies, known as **Service messages**, through the WhatsApp Business Platform.

Until 30 September 2026, these Service messages are free from Meta messaging charges.

From **1 October 2026**, Meta will introduce per-message charging for Service messages.

However, the first **1,000 Service messages per business phone number each month will remain free**.

#### At a glance

| Message Type                                         | Until 30 Sep 2026 | From 1 Oct 2026 |
| ---------------------------------------------------- | ----------------- | --------------- |
| Incoming customer message                            | Free              | Free            |
| First 1,000 Service messages per phone number/month  | Free              | **Free**        |
| Service message after the first 1,000                | Free              | **Charged**     |
| Utility message within 24-hour window                | Free              | **Charged**     |
| Utility message outside 24-hour window               | Charged           | Charged         |
| Marketing message                                    | Charged           | Charged         |
| Authentication message                               | Charged           | Charged         |
| Eligible 72-hour Click-to-WhatsApp free entry window | Free              | Remains free    |

An important distinction is that the **1,000 free monthly allowance applies specifically to Service messages**.

Utility, Marketing and Authentication messages continue to follow their respective Meta pricing rules.

***

### How Does the 1,000 Free Service Message Allowance Work?

Meta will provide the free allowance **per business phone number**, rather than per WhatsApp Business Account.

For example:

**Business Phone Number A**\
1,000 free Service messages per month

**Business Phone Number B**\
1,000 free Service messages per month

If the same business operates three WhatsApp Business phone numbers, each number receives its own monthly Service message allowance.

Charging starts from the **1,001st Service message for each individual phone number**.

The allowance resets each month.

For example, if a business uses only 600 Service messages in October, the remaining 400 messages do not carry over into November.

This also means that businesses with relatively low customer service volumes may continue to incur **little or no Meta Service-message cost** even after the new pricing model takes effect.

***

### The 24-Hour Customer Service Window Still Applies

The introduction of Service message pricing does **not** remove or change the 24-hour customer service window.

When a customer messages your business, the 24-hour window opens.

Every new message from that customer resets the 24-hour window.

During this window, businesses can continue sending normal free-form Service messages.

What changes from 1 October is **how those outgoing Service messages are charged after the monthly free allowance has been used**.

In other words:

**24-hour window = when you are allowed to send Service messages.**

**1,000-message monthly allowance = how many Service messages are free before Meta begins charging.**

***

### Why Is WhatsApp Changing Its Business Messaging Model?

Meta has not provided a specific public explanation for the October Service message pricing change. However, Meta has been progressively introducing measures aimed at improving the quality and relevance of business messaging, including stronger controls around marketing messages, customer opt-ins and the quality of business conversations.

**This forms part of a broader shift toward making business messaging more relevant, intentional and valuable to customers.**

For businesses, this means greater emphasis should be placed on designing conversations that are useful, efficient and purposeful.

***

## Malaysia WhatsApp Messaging Rates From 1 October 2026

Meta has published the rates that will take effect from **1 October 2026**.

For messages delivered to Malaysian recipients:

| Message Category | Meta Rate per Delivered Message     |
| ---------------- | ----------------------------------- |
| Marketing        | **RM0.3467**                        |
| Utility          | **RM0.0564**                        |
| Authentication   | **RM0.0564**                        |
| Service          | **RM0.0564 — same as Utility rate** |

From 1 October 2026, Service messages in Malaysia will follow the applicable Utility rate. The first 1,000 Service messages per business phone number each month are free. The applicable Service rate begins from the 1,001st Service message.

{% hint style="warning" %}
The conversation fees vary based on conversation category and country/region rate. [Click to view the Meta rate card.](https://developers.facebook.com/docs/whatsapp/pricing#rates)
{% endhint %}

#### A Simple Malaysia Example

Suppose one Seampify-connected WhatsApp number sends **1,500 Service messages** during a month.

**First 1,000 Service messages:** Free\
**Remaining 500 Service messages:** 500 × RM0.0564 = **RM28.20**

**Meta Service message charge: RM28.20**

Without the monthly free allowance, 1,500 Service messages at RM0.0564 would amount to RM84.60. However, because the first 1,000 eligible Service messages are free each month, only the remaining 500 messages are charged.

Businesses that stay within the 1,000 free Service messages per phone number each month will not incur Service message charges.

***

## Important: Ensure Your Payment Method Is Set Up Before 30 September 2026

{% hint style="warning" %}
Businesses using the WhatsApp Business Platform should also ensure that a **valid payment method is on file for their WhatsApp Business Account (WABA) by 30 September 2026**.
{% endhint %}

**As your WhatsApp Business Solution Provider, Seampify would like to highlight an important Meta requirement: a valid payment method must be on file for the applicable WhatsApp Business Account(s) by 30 September 2026.**

If no valid payment method is available, Service messages may stop being delivered once Service message charging begins on 1 October 2026.

To avoid any disruption to customer service conversations, you should review and add their payment method **before 30 September 2026**.

**Action required:**

1. Log in to your Meta Business account.
2. Open your WhatsApp Business Account billing/payment settings.
3. Confirm that a valid payment method has been added.
4. If you manage multiple WhatsApp Business Accounts, ensure the required payment setup is completed for each applicable account.

You may refer to Setting up Payment Method guide [here](../../../starting-with-seampify/setting-up-payment-method.md)

This payment requirement relates to **Meta's WhatsApp Business Platform messaging charges** and is separate from your Seampify subscription or platform fees.

**Don't wait until 1 October to complete this setup.** If the payment method is missing when the new charging model takes effect, your business may experience disruption to outgoing Service messages.

***

## What About WhatsApp Coexistence?

For businesses using **WhatsApp Coexistence**, where the same number is connected to both the WhatsApp Business App and the WhatsApp Business Platform/API, there continues to be an important distinction.

### Message sent directly from WhatsApp Business App

**No WhatsApp Business Platform API messaging charge.**

#### Message sent through Seampify / WhatsApp Business API

The message follows Meta's applicable API pricing rules.

For Service messages sent through the Seampify platform, the first 1,000 eligible Service messages per business phone number each month are free, after which the applicable Service rate applies.

### Message sent by chatbot or third-party AI through Seampify

This is also treated as a Service message where applicable and follows the same Service-message pricing model.

Messages sent directly from the WhatsApp Business App remain Business App messages, even when they are synchronised with Seampify through Coexistence.

{% hint style="info" %}
Although messages sent from the WhatsApp Business App may also appear inside the connected platform to keep conversations synchronised, they remain Business App messages and are not converted into chargeable API messages.
{% endhint %}

***

## How Businesses Can Keep WhatsApp Costs Optimised

Businesses with higher conversation volumes should still review how their WhatsApp customer journeys are designed to minimise unnecessary message usage.

The goal is not to reduce customer engagement.

It is to **make every conversation more efficient and every message more valuable**.

### 1. Combine Fragmented Replies

Instead of sending:

> Yes.

> We have stock.

> It's RM250.

> Delivery takes two days.

Consider:

> Yes, the item is currently available at RM250, with delivery typically taking around two working days.

One complete response can provide the same customer experience while reducing unnecessary outgoing messages.

This becomes especially relevant after a business has used its monthly 1,000 free Service messages.

***

### 2. Optimise Chatbot Journeys

Businesses should review chatbot flows that generate many individual replies.

Where appropriate, use:

* buttons;
* list selections;
* structured forms;
* WhatsApp Flows; and
* consolidated chatbot responses.

Instead of asking for customer information across several separate messages, businesses may be able to collect the same information through one structured interaction.

***

### 3. Use Buttons, Lists and WhatsApp Flows

Not every customer interaction requires several back-and-forth messages.

Instead of:

> How can we assist you?

Businesses can provide structured options such as:

**View Products**

**Get a Quote**

**Book an Appointment**

**Speak to Sales**

This helps customers reach their intended action faster while reducing unnecessary conversation steps.

***

### 4. Review Automated Notifications

Businesses should also review recurring automated messages such as:

* order received;
* payment received;
* order processing;
* shipment ready;
* delivery reminder; and
* delivery completed.

Each notification should have a clear customer purpose.

Where appropriate, related updates can be consolidated without reducing the quality of customer communication.

***

### 5. Improve Customer Segmentation

Marketing messages will continue to be charged according to Meta's Marketing rates.

Businesses can improve the return from these messages by sending campaigns to more relevant audiences based on:

* customer interests;
* previous enquiries;
* purchase history;
* location;
* engagement;
* membership status; and
* customer lifecycle.

The objective should not simply be to minimise the number of messages sent.

It should be to improve the **business value generated from every message**.

***

### 6. Make Better Use of Click-to-WhatsApp

Eligible conversations initiated through **Click-to-WhatsApp advertisements or Facebook Page call-to-action buttons** continue to benefit from Meta's **72-hour free entry point window**.

Messages delivered within an eligible free entry point window continue to be free under Meta's applicable rules.

For businesses already using Meta Ads, this makes Click-to-WhatsApp an important consideration when designing customer acquisition journeys.

***

### 7. Track Your Monthly Service Message Usage

With the introduction of the 1,000 free monthly Service messages, businesses should begin monitoring:

* Service messages sent per phone number;
* average Service messages per customer conversation;
* chatbot message volume;
* agent reply volume; and
* which customer journeys generate the most messages.

A business sending **800 Service messages per month** will have a very different cost impact from one sending **20,000 Service messages per month**.

Understanding your actual volume will help you determine where optimisation provides the greatest benefit.

***

## The Goal Isn't Fewer Conversations — It's More Efficient Conversations

With **1,000 free Service messages available per business phone number each month**, businesses with lower Service-message volumes may incur little or no additional Service-message charges.

WhatsApp remains an important channel for customer service, sales and engagement.

Businesses should therefore not respond by simply communicating less.

Instead, the opportunity is to create:

**better-designed conversations, fewer unnecessary messages, smarter automation and more valuable customer interactions.**

At Seampify, we will continue monitoring Meta's WhatsApp Business Platform pricing updates and helping our customers optimise their messaging strategies.

We can also review your existing:

* chatbot journeys;
* AI automation;
* automated notifications;
* customer service workflows; and
* agent messaging practices

to identify opportunities to reduce unnecessary message volume before the new pricing model takes effect.

**If you'd like us to review your existing Seampify automations for the October pricing change, simply let our team know.**

***

## Frequently Asked Questions

<details>

<summary>When does the new pricing take effect?</summary>

The new Service message pricing takes effect on **1 October 2026**.

</details>

<details>

<summary>Are all Service messages immediately charged from 1 October?</summary>

No.

Each business phone number receives **1,000 free Service messages every month**.

Meta only begins charging from the **1,001st Service message** for that phone number during the month.

</details>

<details>

<summary>Do unused free Service messages roll over?</summary>

No.

The 1,000 free Service messages reset monthly and unused messages do not carry forward.

</details>

<details>

<summary>Is the 1,000-message allowance per WABA?</summary>

Meta states that it applies **per business phone number**.

</details>

<details>

<summary>Are incoming customer messages charged?</summary>

No. Incoming messages sent by customers do not incur WhatsApp Business Platform messaging charges.

</details>

<details>

<summary>Will normal agent replies be charged?</summary>

From 1 October 2026, the first **1,000 Service messages per business phone number each month are free**. Meta will charge from the 1,001st Service message onwards at the applicable Service rate.

</details>

<details>

<summary>Will chatbot and AI replies also be charged?</summary>

Service messages sent through chatbots, AI assistants or other API-connected systems follow the same pricing model. The first 1,000 eligible Service messages per business phone number each month are free, with charges applying from the 1,001st message.

</details>

<details>

<summary>Does the 24-hour customer service window still exist?</summary>

Yes.

The 24-hour customer service window still determines when businesses can send normal Service messages.

The change is that Service messages become subject to per-message pricing after the monthly 1,000-message free allowance has been used.

</details>

<details>

<summary>Are Click-to-WhatsApp conversations still free?</summary>

Eligible conversations initiated through Click-to-WhatsApp ads or Facebook Page call-to-action buttons continue to benefit from Meta's **72-hour free entry point window**.

</details>

<details>

<summary>What happens if we use WhatsApp Coexistence?</summary>

Messages sent directly through the **WhatsApp Business App remain free from WhatsApp Business Platform API messaging charges**, even if they are synchronised and visible inside Seampify.

Messages sent through Seampify, chatbot automation or other API-connected systems follow Meta's applicable API pricing rules.

</details>

<details>

<summary>Does this affect the normal WhatsApp Business App?</summary>

The new API Service message charge does not apply to messages sent directly from the WhatsApp Business App.

</details>

<details>

<summary>How should my business prepare?</summary>

Businesses should review their:

* agent messaging habits;
* chatbot flows;
* automated notifications;
* frequently asked questions;
* marketing segmentation;
* Click-to-WhatsApp strategy; and
* overall WhatsApp customer journeys.

The goal should not simply be to send fewer messages.

It should be to **make every conversation more efficient and every message more valuable**.

</details>

***

## Learn More

For the latest information on WhatsApp Business Platform pricing, message categories and market rates, refer to [Meta's official WhatsApp Business Platform pricing page](https://business.whatsapp.com/products/platform-pricing?utm_source=chatgpt.com).

You can also review or [add the payment method](../../../starting-with-seampify/setting-up-payment-method.md) associated with your Meta Business account through Meta's Billing & Payments settings.

As Meta may continue to update its pricing documentation ahead of 1 October 2026, Seampify will continue monitoring these changes and update our customers where necessary.
