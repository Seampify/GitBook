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

With WhatsApp Message Templates, you can stay connected with your customers even after the WhatsApp Business Platform's 24 Hour Customer Service Window.

## What's WhatsApp Message Templates? <a href="#message-templates" id="message-templates"></a>

WhatsApp message templates are used to open marketing, utility, and authentication [conversations](https://developers.facebook.com/docs/whatsapp/pricing#conversations) with customers. Unlike free-form messages, template messages are the only type of message that can be sent to customers who have yet to message you, or who have not sent you a message in the last 24 hours.



**A message template could be a text message regarding support, appointment reminders, payment or shipping updates, alerts, etc.** A business can create its own message templates, which is supported at Seampify as well; however, to send them, they should meet some requirements that are,

* A message template must be approved by WhatsApp before sending. At Seampify, once created the template, you can send it for approval with a single click.
* A message template is for business-initiated conversation; therefore, a customer must have opted-in to receive messages from your business for that type of conversation.

If your Message Template meets these requirements, you can send them without any further action.



## Types of Message Template <a href="#types-of-message-template" id="types-of-message-template"></a>

WhatsApp Business Platform supports 3 message template categories -

### Marketing templates <a href="#marketing-templates" id="marketing-templates"></a>

Marketing templates are Meta's most flexible. They can enable businesses to achieve a wide range of goals, from generating awareness to driving sales and more.

### Utility templates <a href="#utility-templates" id="utility-templates"></a>

Utility templates are typically triggered by a user action or request. They must include specificity about the active or ongoing transaction, account, subscription or interaction to which they relate. For example, an order confirmation must contain an order number.

### Authentication templates

{% hint style="warning" %}
Only authentication templates can be used to send a one-time passcode for identity verification; marketing and utility templates cannot be used for this.
{% endhint %}

Authentication templates enable businesses to authenticate users with one-time passcodes (usually 4-8 digit alphanumeric codes), potentially at multiple steps in the login process (e.g., account verification, account recovery, integrity challenges).

Authentication templates are Meta's most restricted. For a template to be classified as authentication, a business must:

* Use WhatsApp’s preset authentication message templates, which include optional add-ons like security disclaimers and expiry warnings
* Configure a one-time password button (copy-code or one-tap)
* Follow content restrictions: URLs, media, and emojis are not allowed for authentication template content or parameters. Additional length restrictions of 15 characters also apply to parameters.

{% content-ref url="message-templates-example.md" %}
[message-templates-example.md](message-templates-example.md)
{% endcontent-ref %}



## Setting Up a Message Template <a href="#limitations" id="limitations"></a>

Before sending a template message, you need to [create a template](../../../seampifys-modules/settings/more-settings/channels/manage-templates/#create-a-template-messages) and get approved. Refer the below to learn more about creating a template.

{% content-ref url="../../../seampifys-modules/settings/more-settings/channels/manage-templates/" %}
[manage-templates](../../../seampifys-modules/settings/more-settings/channels/manage-templates/)
{% endcontent-ref %}



## How Long until My Template is Approved?

Once a template is submitted, it will be sent to Meta for approval. This process typically only takes a few minutes, but in some cases, it can take up to 24 hours up till 3 days.

{% hint style="warning" %}
Seampify is not involved in the template approval process, but if your template is stuck in pending for more than 24 hours, we can help you create a ticket to Meta to check on the status. Kindly reach out to our support team.
{% endhint %}



## Sending a Message Template&#x20;

There are 3 ways to use a message template,

1. Using [Chat](../../../seampifys-modules/chat/messaging-tools.md)
2. Using [Drip Campaign](../../../seampifys-modules/drip-campaign/create-a-drip-campaign.md)
3. And using [Campaign](../../../seampifys-modules/campaigns/bulk-broadcast-via-campaign.md)

{% hint style="success" %}
If you've created your template and got the approval, you can explore the above links reference to send it.
{% endhint %}



## Limitations of Message Templates <a href="#limitations" id="limitations"></a>

* The message template name field is limited to 512 characters.
* The message template content field is limited to 1024 characters.
* A template can only be edited when it is in a state of **Approved**, **Rejected**, or **Paused**. Approved templates can be edited up to 10 times in a 30 day window, or 1 time in a 24 hour window. Rejected or paused templates can be edited an unlimited number of times.&#x20;
* WhatsApp Business Accounts can only create 100 message templates per hour.
* Templates composed of 4 or more buttons, or a quick reply button and one or more buttons of another type, cannot be viewed on WhatsApp desktop clients. WhatsApp users who receive one of these template messages will be prompted to view the message on a phone instead.
* The number of templates a WhatsApp Business Account can have is determined by its parent business. If a parent business is unverified, each of its WhatsApp Business Accounts is limited to 250 templates. However, if the parent business is [verified](https://www.facebook.com/business/help/1095661473946872) and at least one of its WhatsApp Business Accounts has a business phone number with an approved [display name](https://www.facebook.com/business/help/338047025165344), each of its WhatsApp Business Accounts can have up to 6,000 templates.



## Best Practices for Marketing Templates <a href="#best-practices-for-marketing-templates" id="best-practices-for-marketing-templates"></a>

#### Marketing Opt-Out Button <a href="#marketing-opt-out-button" id="marketing-opt-out-button"></a>

We recommend that you add a [Quick Reply button](https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/components#quick-reply-buttons) to templates categorized as `MARKETING` that makes it easy for customers to opt-out of your marketing messages. This gives your customers the option to opt-out of your marketing messages without having to block your business. As a result, you may be able to scale messaging volume faster. Please refer to [this article](https://www.facebook.com/business/help/448422200528701) for further details on the benefits of adding an opt-out button to your marketing templates.
