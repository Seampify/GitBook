---
icon: message-dollar
---

# WhatsApp Conversation Based Pricing

## Charging Model

The WhatsApp Business Platform uses a **per-message pricing structure**, where each message sent by the business is billed individually. However, service messages sent within the [24-hour customer service window](../understanding-24-hour-customer-service-window.md#id-24-hour-customer-service-window) are free of charge for the first 1,000 messages.

<figure><img src="../../../.gitbook/assets/image (907).png" alt=""><figcaption></figcaption></figure>

## Categories of WhatsApp Conversations

Conversations are categorized with one of the following categories:

1. **User-initiated Conversations:**\
   These are triggered when customers contact a business for support or inquiries.<br>
2. **Business-Initiated Conversations:**\
   Businesses start these interactions through notifications or broadcast messages, which are further divided into three template types:
   * **Marketing Messages:** \
     Enables you to achieve a wide range of goals, from generating awareness to driving sales and retargeting customers. Examples include new product, service, or feature announcements, targeted promotions/offers, and cart abandonment reminders.
   * **Utility Messages:** \
     Enables you to follow-up on user actions or requests. Examples include opt-in confirmation, order/delivery management (e.g., delivery update); account updates or alerts (for example., payment reminder); or feedback surveys.
   * **Authentication Messages:** \
     Enables you authenticate users with one-time passcodes, potentially at multiple steps in the login process (e.g., account verification, account recovery, integrity challenges).
   * **Service Messages:**\
     A message sent by the business in response to a customer within the 24-hour customer service window.<br>
3.  **Free Entry Point Conversations** (**Referral Conversations):**\
    Initiated via:

    * Click-to-Action buttons on Facebook pages; or
    * Click-to-WhatsApp Ads (CTWA)



    **Key Details of Referral Conversations:**

    * Sessions remain active for 24 hours from the last customer message.
    * Businesses can send multiple message template free of charge for up to 72 hours from the time the conversation was initiated, provided they reply within 24 hours of the customer’s initial message.
    * Beyond the 72-hour window, new conversations are charged according to the pricing model.

{% hint style="warning" %}
The conversation triggered by a CTWA Ad is free; however, the cost of the ad itself is not.
{% endhint %}



## How are Conversations being charged? <a href="#how_are_conversations_being_charged" id="how_are_conversations_being_charged"></a>

Charges are determined by the category of the conversation initiated:

* **User-Initiated Conversations**: These are free of charge.
* **Business-Initiated Conversations**: These are chargeable based on the category of the Message Template used and the time it was sent.

The types of Business-Initiated Conversation category and its charges for **Malaysian country code** number is as below:

{% hint style="warning" %}
The conversation fees vary based on conversation category and country/region rate. [Click to view the Meta rate card.](https://developers.facebook.com/docs/whatsapp/pricing#rates)
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (909).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Seampify does not impose any additional charges for conversations. All conversation charges are based solely on Meta's pricing.
{% endhint %}

Charges are applied per per individual message sent. All incoming messages are free.&#x20;

Here’s how it works:

* If you send a **marketing, utility or authentication conversation message template**, you will be charged the fee associated with template category conversations every time.
* If you send an **service conversation message,** you will only be charged the fee associated with service conversations if it's more than 1,000 messages, per month.

{% hint style="warning" %}
Whenever a WhatsApp user messages you, this 24-hour timer (customer service window) starts or refreshes if the WhatsApp user messages you again.
{% endhint %}

