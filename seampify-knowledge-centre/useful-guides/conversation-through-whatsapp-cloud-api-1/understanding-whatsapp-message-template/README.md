---
icon: message-lines
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# Understanding WhatsApp Message Template

WhatsApp Message Templates allow businesses to stay connected with customers even after the 24-hour customer service window has closed.

## What's WhatsApp Message Templates?

WhatsApp message templates are pre-approved messages used for [marketing, utility, and authentication purposes](https://developers.facebook.com/documentation/business-messaging/whatsapp/templates/). Unlike regular messages, approved templates can be sent outside the 24-hour customer service window.

**Message templates can be used for appointment reminders, payment or shipping updates, alerts, promotional messages, and more.**

Businesses can create message templates directly in Seampify. However, the following requirements must be met:

* **Meta approval:** Message templates must be approved by Meta before they can be sent. Once created in Seampify, templates can be submitted for approval.
* **Customer opt-in:** Businesses must obtain appropriate [customer consent](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in) before sending business-initiated messages.

Once a message template is approved and these requirements are met, it can be sent through Seampify.

## Types of Message Template <a href="#types-of-message-template" id="types-of-message-template"></a>

WhatsApp Business Platform supports 3 message template categories -

The WhatsApp Business Platform supports three message template categories:

#### Marketing Templates

Marketing templates help businesses promote products, services, and offers, generate awareness, and encourage customer engagement.

They are commonly used for promotional campaigns, product announcements, and special offers.

#### Utility Templates

Utility templates are typically triggered by a customer's action or request. They provide information related to an existing transaction, account, subscription, or interaction.

For example, an order confirmation should include specific information such as an order number.

#### Authentication Templates

{% hint style="warning" %}
Only authentication templates can be used to send one-time passcodes (OTPs) for identity verification. Marketing and utility templates cannot be used for this purpose.
{% endhint %}

Authentication templates allow businesses to verify users through one-time passcodes, such as during account registration, login, or account recovery.

To create an authentication template, businesses must:

* Use Meta's preset authentication template format, which supports optional security disclaimers and expiry warnings.
* Include a one-time password button, such as **Copy Code** or **One-Tap**.
* Follow Meta's content restrictions. URLs, media, and emojis are not permitted in authentication template content or parameters.

{% content-ref url="message-templates-example.md" %}
[message-templates-example.md](message-templates-example.md)
{% endcontent-ref %}

## Setting Up a Message Template <a href="#limitations" id="limitations"></a>

Before sending a template message, you must [create a message template](../../../seampifys-modules/settings/more-settings/channels/manage-templates/#create-a-template-messages) in Seampify and submit it to Meta for approval.

For detailed instructions, refer to the guide below.

{% content-ref url="../../../seampifys-modules/settings/more-settings/channels/manage-templates/" %}
[manage-templates](../../../seampifys-modules/settings/more-settings/channels/manage-templates/)
{% endcontent-ref %}

## How Long until My Template is Approved?

Once submitted, your message template will be reviewed by Meta. Approval typically takes a few minutes but may take up to 24 hours or longer in some cases.

{% hint style="warning" %}
Seampify is not directly involved in Meta's template approval process. If your template remains pending for more than 24 hours, please contact our support team. We can assist you in raising a support ticket with Meta to check its status.
{% endhint %}

## Sending a Message Template

There are three ways to send an approved message template through Seampify:

1. Using [Chat](../../../seampifys-modules/chat/messaging-tools.md)
2. Using [Drip Campaign](../../../seampifys-modules/drip-campaign/create-a-drip-campaign.md)
3. And using [Campaign](../../../seampifys-modules/campaigns/bulk-broadcast-via-campaign.md)

{% hint style="success" %}
Once your message template has been approved, you can follow the guides above to start sending it through Seampify.
{% endhint %}

## Limitations of Message Templates <a href="#limitations" id="limitations"></a>

WhatsApp message templates are subject to Meta's requirements and limitations:

* **Template name:** Maximum of 512 characters.
* **Template content:** Maximum of 1,024 characters.
* **Editing templates:** Templates can be edited when their status is Approved, Rejected, or Paused. Approved templates can be edited once within 24 hours, up to 10 times within a 30-day period. Rejected or paused templates can generally be edited without these frequency restrictions.
* **Template creation:** A WhatsApp Business Account can create up to 100 message templates per hour.
* **Desktop compatibility:** Templates containing four or more buttons, or certain combinations of quick-reply and other buttons, may not display on WhatsApp desktop clients. Customers may be prompted to view them on their phones instead.
* **Template limits:** Unverified business portfolios can have up to 250 templates per WhatsApp Business Account.

For [verified businesses](https://www.facebook.com/business/help/1095661473946872) with at least one approved WhatsApp Business [display name](https://www.facebook.com/business/help/338047025165344), this limit can increase to 6,000 templates per WhatsApp Business Account.

These limitations are subject to Meta's latest policies and account eligibility requirements.

## Best Practices for Marketing Templates <a href="#best-practices-for-marketing-templates" id="best-practices-for-marketing-templates"></a>

#### Marketing Opt-Out Button <a href="#marketing-opt-out-button" id="marketing-opt-out-button"></a>

We recommend adding a [Quick Reply button](https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/components#quick-reply-buttons) to marketing templates categorised as `MARKETING` so customers can easily opt out of receiving promotional messages.

This gives customers more control over the messages they receive without having to block your business.&#x20;

Providing a clear opt-out option can also help maintain message quality and support healthier customer engagement.&#x20;

For more information, refer to [Meta's guide on marketing opt-out buttons](https://www.facebook.com/business/help/448422200528701).
