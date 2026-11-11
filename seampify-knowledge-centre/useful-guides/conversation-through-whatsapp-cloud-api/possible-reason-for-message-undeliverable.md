---
icon: message-exclamation
---

# Possible Reason for "Message Undeliverable"

When sending template messages to your contacts via Seampify, you may see an error **"Message Undeliverable"**

The message may look like this -

<figure><img src="../../.gitbook/assets/image (636).png" alt="" width="536"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (637).png" alt=""><figcaption></figcaption></figure>

## **Possible Reasons**

The following scenarios can cause a message to appear as sent but not delivered. For many of these reasons, Meta will not disclose the underlying cause of the error, due to privacy and policy reasons. This error may occur due to one of these reasons -

* The recipient phone number is not a WhatsApp phone number.
* Recipient Phone Number has blocked your business.
* The recipient did not come online during the 30 day window where Meta hold messages for offline users.
* Recipient has not accepted WhatsApp's new Terms of Service and Privacy Policy.
* Recipient using an old WhatsApp version; must use the following WhatsApp version or greater:
  * Android: 2.21.15.15
  * SMBA: 2.21.15.15
  * iOS: 2.21.170.4
  * SMBI: 2.21.170.4
  * KaiOS: 2.2130.10
  * Web: 2.2132.6
* The message was not delivered to create a high quality user experience. WhatsApp imposes a max limit of marketing template messages that a contact can receive in a certain time across all businesses. You can read more about this here - [Per-User Marketing Template Message Limits](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates#per-user-marketing-template-message-limits).
* Recipient Phone Number is in a [restricted or sanctioned country](https://developers.facebook.com/docs/whatsapp/cloud-api/support#country-restrictions).
* Recipient Phone Number is part of an [experiment](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/experiments) group.



## How to solve this?

To resolve this issue, using a non-WhatsApp communication method (e.g., email, SMS, or phone call), ask the WhatsApp user to:

* confirm that they can actually send a message to your WhatsApp business phone number(s)
* confirm that none of your WhatsApp business phone numbers are in their list of blocked numbers (**Settings** > **Privacy** > **Blocked** or **Blocked contacts**)
* confirm that they have accepted our latest Terms of Service (**Settings** > **Help**, or **Settings** > **Application information** will prompt them to accept the latest terms/policies if they haven't done so already)
* update to the latest version of the WhatsApp app

