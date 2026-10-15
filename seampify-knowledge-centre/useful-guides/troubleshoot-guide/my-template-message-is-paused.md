# My Template Message is Paused

## Template Pacing <a href="#template-pacing" id="template-pacing"></a>

{% hint style="warning" %}
Starting April 30, 2024, template pacing applies to both marketing and utility templates.
{% endhint %}

Template pacing is a mechanism that allows time for customers to provide early feedback on templates. This identifies and pauses templates that have received poor feedback or engagement, giving you enough time to adjust their contents before they are sent to too many customers, thereby **reducing the likelihood of negative feedback impacting your business.**

Template pacing is valid for marketing and utility templates. Newly created templates, paused templates that are unpaused, and templates that may have been created previously but don’t have a GREEN quality rating are potentially subject to pacing. Template quality history — for example, low quality resulting in a template pause — is one of the primary reasons for template pacing and you may see other templates get paced.

When a template is paced, messages will be sent normally until an unspecified threshold is reached. Once this threshold is reached, subsequent messages using that template will be held to allow enough time for customer feedback. Once we receive a good quality signal, subsequent messages using that template will be scaled to the entire target audience. If we receive a bad quality signal, subsequent messages using that template will be dropped, giving you the opportunity to adjust content, targeting, etc.



## Utility Template Pacing&#x20;

Utility templates are subject to pacing only if you have had a utility template paused. Once a utility template has been paused, newly created templates, paused templates that are unpaused, and templates that may have been created previously but don’t have GREEN quality rating are potentially subject to pacing for the next 7 days.



## Template Pausing <a href="#template-pausing" id="template-pausing"></a>

If a message template reaches the lowest quality rating (a status of **Active - Low quality**), it will automatically be paused for a period of time to protect the quality rating of phone numbers that have used the template. Pausing durations are as follows:

* 1st Instance: **Paused** for 3 hours
* 2nd Instance: **Paused** for 6 hours
* 3rd Instance: **Disabled**

When a message template is paused (status of **Paused**) it can't be sent to customers, so you should halt any automated messaging campaigns that rely on that template. Although you won't be charged for attempting to send a paused message template to a customer, and the attempt won't count against your [messaging limit](../broadcasting-through-whatsapp-cloud-api/broadcast-messaging-limit.md), the API will reject these attempts anyway. You should only resume these campaigns when the template's status has been set to **Active** again.

You may wish to edit a paused template if you feel that editing its content will reduce the amount of negative feedback it may receive and increase user engagement. Keep in mind, however, that once you edit a message template and resubmit it for approval, its status will change to **In Review** and it can't be sent to customers again until it has been re-approved and its status set to **Active**.

You may also wish to make changes to your business logic (targeting, delivery parameters, etc.) if you feel it is contributing to negative feedback or low engagement.

Pausing will initially not impact the business phone number from which the message template was sent, or cause the phone number's message limit to decrease. Other high quality message templates can continue to be sent from the phone number. However, if a business consistently sends message templates that reach a **Low quality** status, the phone number may eventually be impacted.



## Pause Notifications <a href="#pause-notifications" id="pause-notifications"></a>

When a message template has been paused we will notify you by WhatsApp Manager notification, email, and webhook if you are subscribed to message template change webhooks. See [Monitoring Status Changes](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#monitoring-status-changes) for webhook setup information and [Examples - Template Paused](https://developers.facebook.com/docs/whatsapp/business-management-api/webhooks/components#template-paused) for a sample webhook payload.



## Unpausing <a href="#unpausing" id="unpausing"></a>

A template will unpause on its own after satisfying the pause duration outlined above. Once unpaused, the template's status will be set to **Active** and you may begin sending it to customers again. If you didn't halt any automated messaging campaigns that relied on a paused template, they should start working again. However, we recommend that you halt any campaigns that rely on a template that has been paused until it is unpaused, because our APIs will reject your requests anyway.

The template's quality rating will also be reset to a value based on the most recent customer feedback the template has received.

Similar to pause notifications, we will notify you by WhatsApp Manager notification, email, and webhook once the template's status has been set to **Active**.



## Appeals <a href="#appeals" id="appeals"></a>

If your submission is rejected you may file an appeal. Note that appeals must [include a sample](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#samples). If an approved template has become disabled, you may also [edit](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#editing) it and resubmit it for approval.

In the **WhatsApp Manager**:

1. Mouseover the suitcase icon (**Account tools**) and click **Message templates**.
2. If you have multiple WhatsApp Business Accounts, use the dropdown menu in the top-right corner to select the account whose templates you want to manage.
3. Find the message template that you would like to edit and click it.
4. Edit the template's contents.
5. Click the **Add Sample** button and add sample variable values and images.
6. Click **Submit**.

The appeal will be reviewed and a decision made within 24 hours.
