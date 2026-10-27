# Manage Templates

{% embed url="https://youtu.be/3IHbSdnsZ1I" %}

Message Templates are used to initiate a conversations after the [24-hour Customer Service Window](../../../../../useful-guides/conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md).

To access the Message Template for the Cloud API WhatsApp Channel, go to **Settings** → **Channels** → then click on the **Manage Templates** tab under the Channel.

<figure><img src="../../../../../.gitbook/assets/image (617).png" alt=""><figcaption></figcaption></figure>

This will open the Message Templates window.

<figure><img src="../../../../../.gitbook/assets/New Template UI (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

The options available are under the ![](<../../../../../.gitbook/assets/image (157).png>) :

* **Create WhatsApp Template** - Using this, you can access the builder to create a WhatsApp Message Template.
* **Synchronize with Facebook** - Sync Seampify Templates with your WhatsApp Account.
* **Delete the Message Template** <img src="https://docs.rampwin.com/~gitbook/image?url=https%3A%2F%2Ffiles.gitbook.com%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FhElFPtMZjXYjDDMBT5q2%252Fuploads%252F3Of4IVOBkTD6Yfey20F7%252FDelete%2520Button.png%3Falt%3Dmedia%26token%3D82c696d8-8f39-4ebd-82c3-f74f28e61d38&#x26;width=28&#x26;dpr=4&#x26;quality=100&#x26;sign=9f9e0612&#x26;sv=2" alt="" data-size="line">
* **Edit the Message Template** <img src="../../../../../.gitbook/assets/image (620).png" alt="" data-size="line">
* **Duplicate the Message Template** <img src="../../../../../.gitbook/assets/image (621).png" alt="" data-size="line">
* **Copy Template JSON** <img src="../../../../../.gitbook/assets/image (622).png" alt="" data-size="line">
* **Create Automation Workflow** ![](<../../../../../.gitbook/assets/image (162).png>) - You can directly create an automation based on the template message that you have setup. A more straightforward method compared to using callback IDs.\
  You may find a guide to set this up through - [here](create-automation-from-templates.md).
* **View insights** <img src="../../../../../.gitbook/assets/image (623).png" alt="" data-size="line"> - Hover over the template message to view the Template Analytics where you can check on the send status and read status by date range as well as the amount spen&#x74;**.**

<figure><img src="../../../../../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

## Create a Template Messages

{% stepper %}
{% step %}
To create a Message Template, click "+ Create Whatsapp Template" button.

<figure><img src="../../../../../.gitbook/assets/CreateTempalte (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
A Create Message Template popup will come in.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2Fb5Xf6Ge748S6TZVORoeH%2Fimage.png?alt=media&#x26;token=1bfbc4cf-c3e8-4e86-944c-1b0535d127f9" alt=""><figcaption></figcaption></figure>

Overview of Create Message Template popup:

* **Name -** Define Template Name. Each Template Name is unique, this means you are unable to create more than one template with the same name.
* **Category** - Select between Marketing, Utility or Authentication. [Check out Message Template to learn more.](../../../../../useful-guides/conversation-through-whatsapp-cloud-api-1/understanding-whatsapp-message-template/#types-of-message-template)
* **Language -** Choose language. Ensure you select the language in which you'll add the body text. Otherwise, it will be rejected.

{% hint style="danger" %}
You can add another language in your content, but it must not exceed 50% of the chosen language. If it does, it may be rejected.
{% endhint %}

* **Template** - Set template, choose between Standard, Catalog, Multi-product message or Carousel.
* **Header -** Select header options : None, Text, Image, Video or Document.
* **Body -** Add body text. You may use Variable that will be used as a placeholder for the template.
* **Footer (Optional) -** Set footer message.
* **Button (Optional) -** Add button options. This is mandatory for Carousel template.

{% hint style="danger" %}
Emojis cannot be used in buttons. You are unable to submit for approval if button contains emoji.
{% endhint %}

{% hint style="info" %}
For **marketing messages**, Meta recommends adding an unsubscribe option. To do so, include this in the footer by typing: **Reply "STOP" to unsubscribe.** This will automatically remove the contact from your future broadcast list. Refer to the [Broadcast Subscription Automation Guide](../../../../automations/import-automation-template/#broadcast-subscription-automation-guide).
{% endhint %}
{% endstep %}

{% step %}
After adding all the details to the template, check its Preview, and if everything's fine, click **Submit For Approval**.

<figure><img src="../../../../../.gitbook/assets/image (630).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
You will see the newly created template message in the page and the status will be Pending. Approval typically takes **10–30 minutes**. Once approved, you may send the template.

<figure><img src="../../../../../.gitbook/assets/Approval.png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

### Types of Headers in Message Template <a href="#step-2-perform-a-campaign" id="step-2-perform-a-campaign"></a>

If you choose Header type as **Text**, you may add a bolded text before your body text.

If you choose Header type as **Image**, **Video**, or **Document**, you need to upload a sample file to help Meta verify the use. It should be a sample file, not an original Image, Video, or Document detailing your contact.

<figure><img src="../../../../../.gitbook/assets/image (626).png" alt="" width="563"><figcaption></figcaption></figure>

### Using Variable in Message Template <a href="#step-2-perform-a-campaign" id="step-2-perform-a-campaign"></a>

If you choose add a variable, you may use it as a placeholder for the template, which you'd replace with the correct information of the contact you'll send the template to. Plus, add the variable's example in the **Sample for body content** field.

<figure><img src="../../../../../.gitbook/assets/image (625).png" alt=""><figcaption></figcaption></figure>

For instance, if you'd replace the variable placeholder with the contact's name, you can enter example content as Name to help Meta verify the use of the template and approve it.

{% hint style="info" %}
If you set body text as, "_Hi \{{1\}}, your parcel is on the way to you_," and Example content for \{{1\}} as "_Name_," then while sending the template message to the contact, replace variable to contact's name. The template body text would be, "_Hi **Alex,** your parcel is on the way to you._"
{% endhint %}

### Footer in Message Template

If you'd like to add a Footer to the template, you can do that in the Footer Field, which is optional.

{% hint style="info" %}
For **marketing messages**, Meta recommends adding an unsubscribe option. To do so, include this in the footer by typing: **Reply "STOP" to unsubscribe.** This will automatically remove the contact from your future broadcast list. Refer to the [Broadcast Subscription Automation Guide](../../../../automations/import-automation-template/#broadcast-subscription-automation-guide).
{% endhint %}

### Button(s) in Message Template

After the footer, you get the option to add buttons to your message template. The template support adding two types of buttons: **Call to Action** and **Quick Reply**.

<figure><img src="../../../../../.gitbook/assets/image (627).png" alt="" width="225"><figcaption></figcaption></figure>

The Call to Action button lets you further add 2 buttons:

* **Call Phone Number** - direct user to call the number using telco line from their mobile.
* **Visit Website** - direct user to an external website.

<figure><img src="../../../../../.gitbook/assets/image (628).png" alt="" width="563"><figcaption></figcaption></figure>

And the Quick Reply button lets you add up to 10 buttons for the selected purpose.

<figure><img src="../../../../../.gitbook/assets/image (629).png" alt="" width="563"><figcaption></figcaption></figure>

## Sending a Message Template

There are 3 ways to use a message template,

1. Using [Chat](../../../../chat/messaging-tools.md)
2. Using [Drip Campaign](../../../../drip-campaign/create-a-drip-campaign.md)
3. And using [Campaign](../../../../campaigns/bulk-broadcast-via-campaign.md)

While using the template through one of the above methods, ensure you replace the variable with the correct information. Simply select the **Attribute Placeholder** to replace the variable. And once you send the template, the message will pick the correct information, and it will look like the following.

<figure><img src="../../../../../.gitbook/assets/template.gif" alt=""><figcaption></figcaption></figure>
