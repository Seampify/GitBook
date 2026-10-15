# Interactive Messages

Using the Buttons/Options/Product Messages (Interactive Messages) option in the WhatsApp channel, send pre-built interactive messages like Buttons, Lists, and Single or Multi Product messages.



To access the Interactive Message for the Cloud API WhatsApp Channel, go to **Settings** → **Channels** →  then click on the **Interactive Messages** tab under the Channel.

<figure><img src="../../../../.gitbook/assets/image (659).png" alt=""><figcaption></figcaption></figure>



## Create an Interactive Message

{% stepper %}
{% step %}
Click on the **+** **Create Interactive Message** button.&#x20;

<figure><img src="../../../../.gitbook/assets/image (660).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Upon clicking, it will open the Create Interactive Message Template builder, where you can define the template name and then select a Message Type.

<figure><img src="../../../../.gitbook/assets/image (662).png" alt=""><figcaption></figcaption></figure>

There are a few Message Types, and upon selecting each of them, you'd get different options.

* [Text](interactive-messages.md#text)
* [Buttons/Flow](interactive-messages.md#buttons-flow)
* [List](interactive-messages.md#list)
* [Address](interactive-messages.md#address)
* [Location](interactive-messages.md#location)
* [Single Product](interactive-messages.md#single-product) (only available if you've set your Catalog)
* [Multi Products](interactive-messages.md#multi-products) (only available if you've set your Catalog)
{% endstep %}

{% step %}
Fill in the **Body Text** with your desired message.&#x20;

You can also use **insert** **Body Placeholder** to personalize the content dynamically.

For example, if you set your Body Text as _"Hi {full\_name}, your order is confirmed."_ When you send the Interactive Message Template, it will automatically replace the placeholder with the recipient's details, such as _"Hi **Alex**, your order is confirmed."_

<figure><img src="../../../../.gitbook/assets/placeholder.gif" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Click **Save** once done and you will see the newly created Interactive Message appears in the list as below.&#x20;

<figure><img src="../../../../.gitbook/assets/image (663).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}



## List of Message Types

There are multiple message types. By default, you will see the first 4 options only. If you have set your Catalog, you have additional option of Single Product and Multi Products options.

* [Text](interactive-messages.md#text)
* [Buttons/Flow](interactive-messages.md#buttons-flow)
* [List](interactive-messages.md#list)
* [Address](interactive-messages.md#address)
* [Location](interactive-messages.md#location)
* [Single Product](interactive-messages.md#single-product)
* [Multi Products](interactive-messages.md#multi-products)

<figure><img src="../../../../.gitbook/assets/image (669).png" alt=""><figcaption><p>Message Type Options</p></figcaption></figure>

### Text

This is the standard message type with text only or text with attachment content.&#x20;

<figure><img src="../../../../.gitbook/assets/image (664).png" alt="" width="563"><figcaption></figcaption></figure>



### Buttons/Flow

This is the message type that contains up to 3 button(s).

<figure><img src="../../../../.gitbook/assets/image (665).png" alt="" width="563"><figcaption></figcaption></figure>

* **Header Type** - Choose to add a Text (a bolded headline before your Body text), attach an Image, Video or Document if desired.

<figure><img src="../../../../.gitbook/assets/image (666).png" alt="" width="563"><figcaption></figcaption></figure>

* **Body Text** - Insert your body content here. You can also use **Insert** **Body Placeholder** which will get replaced with the correct information when you send the template.
* **Footer (Optional)** - Add a footer text (a smaller font size text after Body Text) if desired.
* **Buttons** - Choose to add:
  * Quick Reply - A general button option that can trigger a specific automation when clicked.&#x20;
  * Call To Action - Directs the user to an external website when clicked.
  * or WhatsApp Flow - Loads a designated WhatsApp Form when clicked.

{% hint style="info" %}
Quick Reply button can have up to 3 options but Call to Action and WhatApp Flow button can only have 1 option.
{% endhint %}



### List

This is the message type that contains a button that loads a list of up to 10 options.

<figure><img src="../../../../.gitbook/assets/image (667).png" alt=""><figcaption></figcaption></figure>

* **Header Type** - Choose to add a Text (a bolded headline before your Body text), attach an Image, Video or Document if desired.

<figure><img src="../../../../.gitbook/assets/image (666).png" alt="" width="563"><figcaption></figcaption></figure>

* **Body Text** - Insert your body content here. You can also use **Insert** **Body Placeholder** which will get replaced with the correct information when you send the template.
* **Footer (Optional)** - Add a footer text if desired. This appears in a smaller font below the Body Text.
* **List CTA Label** - Enter the name of the button that will load the list options.

{% hint style="warning" %}
List CTA Label should be less than 20 characters.
{% endhint %}

* **Section Title (Optional)** - Categorize your list by adding a title for each section. Use the **+** button to add more section titles.
* **Section Row Title** - Provide a title for each option displayed to the user. Click + to add more section row.

{% hint style="warning" %}
Section Row Title should be less than 20 characters.
{% endhint %}

* **Section Row Description (Optional)** - Add a description for each option if desired.
* **Callback ID (Optional)**  - Specify an internal **ID** for the button, which can be used to trigger specific automations within the system.

<figure><img src="../../../../.gitbook/assets/image (668).png" alt="" width="361"><figcaption><p>Example of a List option with Section Title</p></figcaption></figure>

{% hint style="danger" %}
You can include a maximum of **10 options** across all sections, regardless of the number of sections you create.
{% endhint %}



### Address

<figure><img src="../../../../.gitbook/assets/image (670).png" alt=""><figcaption></figcaption></figure>

### Location

This is the message type that collect the location of your contacts.

<figure><img src="../../../../.gitbook/assets/image (671).png" alt=""><figcaption></figcaption></figure>

**Body Text** - Enter your message prompting the user to share their location, e.g., _"Click to share your location."_ This will generate a message with a button that, when clicked, opens the user's map in WhatsApp, allowing them to easily share their location.

<figure><img src="../../../../.gitbook/assets/IMG_6E4AF77EABC6-1.jpeg" alt="" width="375"><figcaption><p>Example of a location message type</p></figcaption></figure>

Once a user click on the **Send location** button, it will loads their map and they are able to choose their location to share with you.

<figure><img src="../../../../.gitbook/assets/IMG_6119689AC79F-1.jpeg" alt="" width="375"><figcaption><p>WhatsApp map opened upon clicking the button</p></figcaption></figure>



### Single Product

This is the message type that send a single product catalog to your contact.

<figure><img src="../../../../.gitbook/assets/image (672).png" alt=""><figcaption></figcaption></figure>

* **Body Text** - Insert your body content here. You can also use **Insert** **Body Placeholder** which will get replaced with the correct information when you send the template.
* **Footer (Optional)** - Add a footer text if desired. This appears in a smaller font below the Body Text.
* **Add/Change A Product** - Select the single product you want to send with the message. This allow your contact to view the product's details and add to cart based on the quantity they desire.



### Multi Products

This is the message type that send multiple products catalog to your contact.

<figure><img src="../../../../.gitbook/assets/image (673).png" alt=""><figcaption></figcaption></figure>

* **Text** - Insert a headline for your message. You can also use **Insert** **Body Placeholder** which will get replaced with the correct information when you send the template.
* **Body Text** - Insert your body content here. You can also use **Insert** **Body Placeholder** which will get replaced with the correct information when you send the template.
* **Footer (Optional)** - Add a footer text if desired. This appears in a smaller font below the Body Text.
* **Add Category (Optional)** - Click to add a category of your product(s) if desire. Click **Add Category** to add more category.
* **Add Products** - Select the product(s) you want to send with the message. This allow your contact to view the product options and its details, choose the quantity for each product, then add to cart.

<figure><img src="../../../../.gitbook/assets/image (674).png" alt="" width="375"><figcaption></figcaption></figure>

When you send your contacts the multi product message, they interact with it like the below.

<figure><img src="../../../../.gitbook/assets/image (675).png" alt=""><figcaption></figcaption></figure>



## How to send an Interactive Message

Through [Chat Module](../../../chat/messaging-tools.md#send-buttons-options-product-messages), you can use an interactive message easily.

{% content-ref url="../../../chat/messaging-tools.md" %}
[messaging-tools.md](../../../chat/messaging-tools.md)
{% endcontent-ref %}



## Edit or Delete an Interactive Message

To edit and delete a particular interactive message template,

* Click on the<img src="https://docs.rampwin.com/~gitbook/image?url=https%3A%2F%2Ffiles.gitbook.com%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FhElFPtMZjXYjDDMBT5q2%252Fuploads%252FtM0TpJ2uFQAN4Ck2pMsa%252FEdit%2520Button%2520Blue.png%3Falt%3Dmedia%26token%3De5fd4863-2e0e-4e4c-9854-bca693646d06&#x26;width=38&#x26;dpr=4&#x26;quality=100&#x26;sign=1b3f5130&#x26;sv=2" alt="" data-size="line">Edit Icon button to edit it.
* Or click on the<img src="https://docs.rampwin.com/~gitbook/image?url=https%3A%2F%2Ffiles.gitbook.com%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FhElFPtMZjXYjDDMBT5q2%252Fuploads%252F3Of4IVOBkTD6Yfey20F7%252FDelete%2520Button.png%3Falt%3Dmedia%26token%3D82c696d8-8f39-4ebd-82c3-f74f28e61d38&#x26;width=28&#x26;dpr=4&#x26;quality=100&#x26;sign=9f9e0612&#x26;sv=2" alt="" data-size="line">Delete Icon button to delete the template.
