---
icon: message-exclamation
---

# Common Message Template Rejection Reasons

## Common Rejection Reasons <a href="#common-rejection-reasons" id="common-rejection-reasons"></a>

Message templates may be rejected by Meta for the following reasons. Make sure to avoid these common mistakes when creating your templates.

* **Incorrect variable format:** Variable parameters are missing or have mismatched curly braces. The correct format is `{{1}}`.
* **Invalid variable parameters:** Variables contain unsupported special characters or formatting, such as a `#`, `$`, or `%`.
* **Non-sequential variables:** Variable parameters are not numbered in sequence. For example, `{{1}}`, `{{2}}`, `{{4}}` are used, but `{{3}}` is missing.
* **Too many variables:** The template contains too many variable parameters relative to its message length.
* **Incorrect variable placement:** A variable parameter appears at the beginning or end of the message.
* **Commerce Policy violations:** The template contains content that violates [Meta's Commerce Policy](https://whatsappbusiness.com/policy/), including the promotion or sale of prohibited goods and services.
* **Business Policy violations:** The template violates the [WhatsApp Business Messaging Policy](https://whatsappbusiness.com/policy/), such as requesting sensitive information, including full payment card numbers, financial account numbers, or national identification numbers.
* **Abusive or threatening content:** The template contains threatening, abusive, or harassing language.
* **Duplicate templates:** The template contains the same content as an existing template. Duplicate detection may vary by template type.
* **Unsupported links:** The template contains URL shorteners or links that do not meet Meta's requirements.

If your template is rejected, you can check the rejection reason in [Meta Business Support Home](https://business.facebook.com/business-support-home) or WhatsApp Manager.&#x20;

To view rejected templates in Business Support Home, navigate to **Account Overview > View My Accounts > (Your Meta Business Account) > (Your WhatsApp Business Account (WABA)) > Rejected Message Templates**.

You may also receive an email notification containing the rejection details.

For duplicate templates, the Business Support Home notification may display the name and language of the existing template with identical content. Once you've identified the issue, you can edit the template and resubmit it for approval.

**Note:** Duplicate-template restrictions do not apply to templates categorised as [`AUTHENTICATION`](./#types-of-message-template).&#x20;

## Troubleshooting a Rejected Message Template

You can edit and resubmit a rejected template through the [Manage Templates](../../../seampifys-modules/settings/more-settings/channels/manage-templates/) page in Seampify.&#x20;

Once resubmitted, the template's status will change to **Pending** while Meta reviews it. The template cannot be sent to customers until it has been approved and is active.

## Quality Rating <a href="#quality-rating" id="quality-rating"></a>

Every message template has a quality rating based on customer feedback, engagement, and message performance.

Templates with an **Active** status may display the following quality ratings in WhatsApp Manager:

* **Active – Quality pending** (Green)
* **Active – High quality** (Green)
* **Active – Medium quality** (Yellow)
* **Active – Low quality** (Red)

Newly approved templates generally begin with a **Quality pending** rating.

If a template receives repeated negative feedback, low engagement, or customer complaints, its quality rating may decrease.

Templates with an **Active** status can generally still be sent, although low-quality templates may be subject to pacing or restrictions. If Meta changes the template's status to **Paused** or **Disabled**, it cannot be sent until the restriction is resolved and the template becomes active again.

To maintain good template quality, send relevant messages to customers who have opted in and avoid sending excessive or unwanted messages.
