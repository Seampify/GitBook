# Sending Messages

There are 3 ways to initiate a conversation with your customers:

* [Direct Conversation via Chat](../seampifys-modules/chat/)
* [Bulk Broadcast via Campaign](sending-messages.md#step-1-create-template-messages)
* [Scheduled a Sequences Messages via Drip Campaign](../seampifys-modules/drip-campaign/create-a-drip-campaign.md)

For this guide, we shall look into **Bulk Broadcast via Campaign.**

## Step 1: Create Template Messages

Before initiating a conversations, you will need to submit a Template Message to Meta for approval.

{% stepper %}
{% step %}
Go to **Settings > Channels**. Then, click on **Manage Templates** and it will brings you to the Templates Messages page.

<div align="left"><figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FeCvC98XQ6PBZSArkSJ6P%2FScreenshot%202024-12-12%20114110.png?alt=media&#x26;token=a6e5498f-19b0-4443-ad55-e1e5297a09b2" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
Select "+ Create Whatsapp Template" button and it will open a Create Message Template pop up.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FhVNi9I0UHEwoAPodAzz7%2Fimage.png?alt=media&#x26;token=76b67e50-937c-429c-94be-dc9abeff4f64" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Fill in the template details. Once done, click **Submit for Approval**.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2Fb5Xf6Ge748S6TZVORoeH%2Fimage.png?alt=media&#x26;token=1bfbc4cf-c3e8-4e86-944c-1b0535d127f9" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
For **marketing messages**, Meta recommends adding an unsubscribe option. To do so, include this in the footer by typing: **Reply "STOP" to unsubscribe.** This will automatically remove the contact from your future broadcast list. Refer to the [Broadcast Subscription Automation Guide](../seampifys-modules/automations/import-automation-template/#broadcast-subscription-automation-guide).
{% endhint %}
{% endstep %}

{% step %}
Once submitted for approval, you will see the newly created template message in the page and the status will be Pending. Approval typically takes **10–30 minutes**. Once approved, you may send the template message.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2Fq9n5Wm897XfpabMbTuVb%2Fimage.png?alt=media&#x26;token=d4a42e21-1e7a-43f9-ab19-fc66f58cb95a" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Step 2: Perform a Campaign <a href="#step-2-perform-a-campaign" id="step-2-perform-a-campaign"></a>

{% stepper %}
{% step %}
### Start a Campaign <a href="#start-a-campaign" id="start-a-campaign"></a>

After template approval, go to the **Campaign module**. Then, click on "+ **Create Campaign"**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2Fe0rQyUSbsFasJwiZulW9%2Fimage.png?alt=media&#x26;token=e1ba99e3-da79-4adf-a311-ffd4f3a72be5" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Add a Campaign Name <a href="#add-a-campaign-name" id="add-a-campaign-name"></a>

Enter a descriptive **campaign name**, following the DO's and DONT's. Click **Next** to proceed.

<figure><img src="https://lh7-rt.googleusercontent.com/slidesz/AGV_vUfi2v8HhQGn9j10rdti5OQrlUecW4MRQAcZHJ4sV68o8ZuUMy5NWRfARmTjj1JFWn8obm9rSvAKif855117rUsKrV93j6qhMM9W6Hm2bHBsZIlu-ui23PLTupY0FS9zA3Qxc-0MZQsMUmtTk9TSRNl10cHqSYZS=s2048?key=YuKrnlkH4ooGPnQJnGpRUA" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Sender <a href="#select-sender" id="select-sender"></a>

Choose the channel you wish to send from (e.g., WhatsApp, Facebook, Instagram). Then, click **Next**.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FycWitPiLIfjeB70LEygf%2Fimage.png?alt=media&#x26;token=79734dba-d15a-44c7-ad23-66accba398c2" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
With WhatsApp, you can broadcast at any time, whereas on Facebook and Instagram, broadcasts are limited to contacts who have messaged you within 7 days of their initial interaction.
{% endhint %}
{% endstep %}

{% step %}
### Select Contact <a href="#select-contact" id="select-contact"></a>

Here, you can upload your contact list using CSV file or Filter Existing Database.

**Upload Contacts:**

* Click <img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FtL3npYtDC0kw9OqAV9yC%2Fimage.png?alt=media&#x26;token=346afded-38a2-4896-a0f2-f78b5fc6f74a" alt="" data-size="line"> then fill up the informations.

**Filter Existing Database**:

* If broadcasting to a targeted segment, use filters to refine the list. Here, you can filters from the available Contact Fields or Tags that you created in your account.
* Add multiple filters using the **+ button** if needed.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FlFNDhkdVi9YeVClJ9sNS%2Fimage.png?alt=media&#x26;token=5515d59f-f5ce-4bb0-9539-3238d4f04b24" alt=""><figcaption></figcaption></figure>

**Default Behavior:**

* If no filters are applied, the broadcast will be sent to **all contacts** in the system.

After setting the filters, click "Submit" to apply them. The filtered contacts based on your selected criteria will appear at the bottom. If everything looks correct, click "Next" to proceed.
{% endstep %}

{% step %}
### Select Template <a href="#select-template" id="select-template"></a>

Choose the template that was approved by Meta from the dropdown menu. You can also create a new one by click "Create Template" and it will direct you to [Template Message page.](https://app.gitbook.com/s/TDj39bRN1xx5RG7VtqzP/starting-with-seampify/sending-messages#step-1-create-template-messages)​

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FoSGW0b22o2Fd7P60jYSY%2Fimage.png?alt=media&#x26;token=f9adafe8-ca56-4764-9350-b0b56d331519" alt=""><figcaption></figcaption></figure>

If there is a variables in your template message, fill in placeholder variables:

* Use **static data** by entering manually or dynamically capture data from **attributes**.
* For buttons triggering specific actions - Add a **callback ID** to link to specific automation, refer to the Automation Tutorial for Buttons.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FPri0eEN4NyQWpgAh7B0p%2Fimage.png?alt=media&#x26;token=7c42458e-c7c2-43f1-8ba6-a68080f2ea50" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Test Send <a href="#test-send" id="test-send"></a>

Here, you can perform a testing to your number. Select <img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FcMjYAh16KSOqeUTQWfTq%2Fimage.png?alt=media&#x26;token=402b6150-3354-453c-b823-ae4d6ccc391d" alt="" data-size="line"> and you will see a pop out menu to select the contact(s). If your number is not displayed here, you may click + Add Contact.

<div align="left"><figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FTDj39bRN1xx5RG7VtqzP%2Fuploads%2FyxuaosOmtNa5M3t4zLwE%2Fimage.png?alt=media&#x26;token=e3a31efe-ea8f-402f-bba3-a03d918010e7" alt="" width="375"><figcaption></figcaption></figure></div>

It is highly recommended to test before sending the actual bulk broadcast.

{% hint style="info" %}
You can only select a maximum 5 contacts for test send and the selected test send number must not be part of the broadcast contact.
{% endhint %}
{% endstep %}

{% step %}
### Review Campaign <a href="#review-campaign" id="review-campaign"></a>

Check all campaign details carefully. Then choose how you want to send:

#### **Option 1 – Send Now**

Send the campaign immediately to selected contacts.

<figure><img src="../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

***

#### **Option 2 – Set Schedule**

Choose a specific **date and time** to run the campaign once.

![](<../.gitbook/assets/image (128).png>)

***

#### **Option 3 – Periodic (New Feature)**

Automate recurring broadcasts with flexible schedules:

**🔹 Daily**

* Select the **time of day**.
* Choose how often to repeat (e.g., every 1 day, every 2 days).
* Set when the campaign ends (_Never_ or on a specific date).

📸 Example (Daily setup)

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

***

**🔹 Weekly**

* Select the **time of day**.
* Choose how many weeks to repeat (e.g., every 1 week).
* Select the specific weekdays (e.g., Mon, Wed, Fri).
* Set the end condition.

📸 Example (Weekly setup)

<figure><img src="../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

***

**🔹 Monthly**

Choose between **Dates of Month** or **Days of Week**:

1.  **Dates of Month**

    * Pick the exact calendar dates (e.g., 1st, 9th, 16th).
    * Define the end condition.

    📸 Example

<figure><img src="../.gitbook/assets/image (125).png" alt="" width="375"><figcaption></figcaption></figure>

1.  **Days of Week**

    * Select a position (e.g., _First Thursday_, _Second Friday_).
    * Add multiple rules if needed.
    * Define the end condition.

    📸 Example

<figure><img src="../.gitbook/assets/Screenshot 2025-08-25 151903.png" alt="" width="375"><figcaption></figcaption></figure>

***

#### **Retry Campaign**

Enable this option to maximize delivery rates.

* The system will retry up to **3 times automatically** for failed messages.

***

<figure><img src="../.gitbook/assets/image (129).png" alt="" width="375"><figcaption></figcaption></figure>

👉 Click **Send Now** once done and a new campaign will be created.

<figure><img src="../.gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="info" %}
As a reminder, it is recommended to send messages to users who have [opted-in](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in) to receiving messages from you.
{% endhint %}

There are other ways to send messages to your contacts, click to know more.

{% content-ref url="../seampifys-modules/chat/" %}
[chat](../seampifys-modules/chat/)
{% endcontent-ref %}

{% content-ref url="../seampifys-modules/drip-campaign/" %}
[drip-campaign](../seampifys-modules/drip-campaign/)
{% endcontent-ref %}
