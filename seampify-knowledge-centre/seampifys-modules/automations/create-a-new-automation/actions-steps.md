# Actions / Steps

Actions in an automation workflow are the Tasks that get executed when Event activates, and Trigger Condition(s) are fulfilled.



Once you have setup the [Automation Workflow settings](./#step-1-setup-automation-workflow), you will goes to the Automation window. Here, you may click the <img src="../../../.gitbook/assets/image (465).png" alt="" data-size="line"> button or right click on the window to access Action types and add them.

<figure><img src="../../../.gitbook/assets/image (466).png" alt="" width="364"><figcaption></figcaption></figure>

There are quite a number of Actions for the Automated Workflow; based on those, you can run automated tasks at Seampify.

{% hint style="info" %}
If you have integrated to a Marketplace, you will see more Actions node here.
{% endhint %}



## Types of Workflow Action Nodes

There are the different Action Nodes under the below Action Types category which you can use at Seampify:

* [Starting Point Action Types](actions-steps.md#starting-point-actions-types)
* [Workflow Action Types](actions-steps.md#workflow-action-types)
* [Messaging Action Types](actions-steps.md#messaging-action-types)
* [Customer Interaction Action Types](actions-steps.md#customer-interaction-action-types)
* [Security Action Types](actions-steps.md#security-action-types)
* [Technical Action Types](actions-steps.md#technical-action-types)
* [Whatsapp Chat Commerce Action Types](actions-steps.md#whatsapp-chat-commerce-action-types)

To access the nodes' settings, simply double click. Once you have done update the settings, click on <img src="../../../.gitbook/assets/image (491).png" alt="" data-size="line"> to save it.



## **1. Starting Point** Actions Type&#x73;**:**&#x20;

### <img src="../../../.gitbook/assets/image (470).png" alt="" data-size="line">**Trigger Node**

This is your starting point for each Automation Workflow. Under Trigger Node, you may choose your desire Trigger Conditions which is the basis for an automated action(s) to run. There are multiple types of Conditions, which, if fulfilled, the Action(s) will be executed.&#x20;

[Learn more about Trigger Conditions here.](trigger-conditions.md)

<figure><img src="../../../.gitbook/assets/image (467).png" alt="" width="342"><figcaption></figcaption></figure>



## **2. Workflow** Action Type&#x73;**:**

### <img src="../../../.gitbook/assets/image (471).png" alt="" data-size="line">**Criteria Router**

Route the workflow based on specific criteria such as message content, user attributes, or other conditions.

<figure><img src="../../../.gitbook/assets/image (468).png" alt="" width="563"><figcaption></figcaption></figure>

You can set multiple criteria and each criteria can have it's own workflow once the conditions has met, it will look something like this:

<figure><img src="../../../.gitbook/assets/image (469).png" alt="" width="208"><figcaption></figcaption></figure>



### <img src="../../../.gitbook/assets/image (472).png" alt="" data-size="line">**Jump to Automation**

Jump to a specific automation flow automatically.

<figure><img src="../../../.gitbook/assets/image (473).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
You need to have more than one automation running to view the options in the dropdown menu.
{% endhint %}



### <img src="../../../.gitbook/assets/image (474).png" alt="" data-size="line">**Delay Execution**

Introduce delays where necessary to control the timing of actions automatically.&#x20;

<figure><img src="../../../.gitbook/assets/image (475).png" alt="" width="563"><figcaption></figcaption></figure>



## 3. Messaging Action Types:

### <img src="../../../.gitbook/assets/image (476).png" alt="" data-size="line">**Auto Reply Template Message**

If you've created a WhatsApp Template Message and want to send it automatically based on Trigger and its Condition, you can use the **Auto Reply Template Message** in the Workflow Step. This Automation only works for WhatsApp Official API Channels:

<figure><img src="https://docs.rampwin.com/~gitbook/image?url=https%3A%2F%2F290002001-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FURHq2UUVreYyIs2nEwlr%252Fuploads%252F1L2fc78wsL3VheonXqsj%252Fimage.png%3Falt%3Dmedia%26token%3De7de683e-3eee-440a-a148-3f3efc0d1df1&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=a7fe571b&#x26;sv=2" alt="" width="563"><figcaption></figcaption></figure>

* Click on the Add Workflow Step **→** then select **Auto Reply Template Message** in the Action Type.
* After selecting the action type, select the template you've created before.
* Then, preview your message template and click **Add**.

{% hint style="warning" %}
WhatsApp Message Template is chargeable based on the category. Refer to the WhatsApp API Conversation-Based Pricing
{% endhint %}



### <img src="../../../.gitbook/assets/image (478).png" alt="" data-size="line">**Auto Reply Button/Option/Products**

Send automated replies that include attachments, buttons for options/WhatsApp Flow and/or ask for location.&#x20;

<figure><img src="../../../.gitbook/assets/image (479).png" alt="" width="563"><figcaption></figcaption></figure>

If you've created Product Catalogs in the WhatsApp Store Settings, you will see the options to see Single Product or Multi Products options.

<figure><img src="../../../.gitbook/assets/image (480).png" alt="" width="534"><figcaption></figcaption></figure>



### <img src="../../../.gitbook/assets/image (481).png" alt="" data-size="line">**Auto Reply and Collect User Inputs**

If you want to ask users bot questions and want to save their responses in the contact fields automatically, you can use this Action Node.

<figure><img src="../../../.gitbook/assets/image (482).png" alt=""><figcaption></figcaption></figure>

In this setup, you need to define a question in the **Question** field. For the answer, select a **Contact Field** from the **Save To** option to store the user's response. The dropdown menu will display the available Contact Fields in your Seampify account. If the desired option is not listed, you can [create a new Contact Field.](../../contacts/filter-options/contact-fields.md#create-a-contact-field)

<figure><img src="../../../.gitbook/assets/image (483).png" alt="" width="375"><figcaption></figcaption></figure>

{% hint style="warning" %}
If you save the anwer on a **Tag** and **Remark** Contact Field, it will replace the existing data with the new data by user's response. [Refer Add Tag Action Node instead](actions-steps.md#add-tags)  if you wish to add on to the existing Tag.
{% endhint %}



You can also validate the responses you wish to collect. The available validation types are as follows:

<figure><img src="../../../.gitbook/assets/image (485).png" alt="" width="563"><figcaption></figcaption></figure>

If you have multiple button options and want to collect only responses from the buttons, select **Interactive** as the Validation Type. Additionally, include a rejection message to notify the contact if they provide an answer outside of the button options.

<figure><img src="../../../.gitbook/assets/image (486).png" alt="" width="563"><figcaption></figcaption></figure>



## 4. Customer Interaction Action Types:

### <img src="../../../.gitbook/assets/image (487).png" alt="" data-size="line">**Add To Drip Campaign**

If you've created a Drip Campaign and want to add a contact into that campaign automatically based on Trigger and its Condition, you can use the **Add To Drip Campaign** in the Workflow Step.&#x20;

<figure><img src="../../../.gitbook/assets/image (488).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
You need to [set up Drip Campaign first](../../drip-campaign/#creating-a-drip-campaign) to view the options in the dropdown menu.
{% endhint %}



### <img src="../../../.gitbook/assets/image (489).png" alt="" data-size="line">**Remove From Drip Campaign**&#x20;

If the contact is in a Drip Campaign, and if you want to remove it from that based on the Trigger Condition(s) fulfillment automatically, you can use this particular Action Node.

<figure><img src="../../../.gitbook/assets/image (490).png" alt="" width="563"><figcaption></figcaption></figure>



### <img src="../../../.gitbook/assets/image (492).png" alt="" data-size="line">**Add Contact List**

The automation Workflow can add the contact to a list under this Action Node when the automation trigger is activated.&#x20;

<figure><img src="../../../.gitbook/assets/image (493).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
This is helpful for categorizing new leads into their respective lists for better organization.
{% endhint %}



### <img src="../../../.gitbook/assets/image (494).png" alt="" data-size="line">**Set Contact Attribute**

If you like to save a message under a specific [Contact Field](../../contacts/filter-options/contact-fields.md) automatically, you can use this Set Contact Attribute Action Node.

<figure><img src="../../../.gitbook/assets/image (495).png" alt="" width="563"><figcaption></figcaption></figure>

You can also update multiple Contact Attribute by clicking the + button. If you couldn't find your desire Contact Attribute from the drop down options, you may [create a new Contact Field here.](../../contacts/filter-options/contact-fields.md#create-a-contact-field)

{% hint style="info" %}
This is useful to update a contact profile field with your dedicated message.
{% endhint %}

{% hint style="warning" %}
If you use **Set Contact Attribute** on a **Tag** and **Remark** Contact Field, it will replace the existing data with the new data you save. [Refer Add Tags action node instead](actions-steps.md#add-tags) if you wish to add on to the existing Tag.
{% endhint %}





<img src="../../../.gitbook/assets/image (496).png" alt="" data-size="line">**Set Conversation Status**

Change the status of a conversation (e.g., open, closed, pending) automatically.

<figure><img src="../../../.gitbook/assets/image (497).png" alt="" width="563"><figcaption></figcaption></figure>



### <img src="../../../.gitbook/assets/image (498).png" alt="" data-size="line">**Mark Blacklisted**

Marking users as blacklisted will automatically prevent further outgoing communication. Once a contact is marked as blacklisted, all automations and broadcast messages via Campaigns or Drip Campaigns will no longer run for that contact.

<figure><img src="../../../.gitbook/assets/image (499).png" alt="" width="173"><figcaption></figcaption></figure>

There is no settings for this Action Node. The contact will be automatically Mark Blacklisted once it goes through this node.

{% hint style="info" %}
This is useful when a contact decides to unsubscribe from your broadcasts, ensuring they no longer receive automated messages or campaigns. Refer to [Broadcast Subscription Automation Guide](../import-automation-template/#broadcast-subscription-automation-guide) for this.
{% endhint %}





### <img src="../../../.gitbook/assets/image (500).png" alt="" data-size="line">**Assign To Team Member**

Assign the contact conversation to users automatically. There are 4 options under this node:

<figure><img src="../../../.gitbook/assets/image (501).png" alt="" width="563"><figcaption></figcaption></figure>

**1. Assign One by One (Round Robin Method)**

* Assigns chats evenly across selected users.
* 💡 _You must first configure the roles to which this rule applies._
* Only users under the selected **Role** will be eligible for assignment.

**2. Assign Department wise (Round Robin Method) ✅&#x20;**_**(Updated)**_

* Assigns chats evenly across users within a selected **Department**.
* 💡 _You must configure Departments under Settings beforehand._

**🆕 Additional Options for Department Assignment:**

When you choose **“Assign Department wise (Round Robin Method)”**, two additional options appear:

* **☑️ Force Reassign Even If Already Assigned To Someone**
  * Reassigns the chat even if it's already assigned to another agent.
* **☑️ Push Chat into Department Queue if Agent is not Available**
  * If no agents are available in the selected department, the chat will be added to the **department queue** instead of failing to assign.

This ensures no customer conversation is missed even when all agents are busy or offline.

{% hint style="info" %}
Proceed to Setting to setup Roles and Department.
{% endhint %}

### <img src="../../../.gitbook/assets/image (503).png" alt="" data-size="line">**Unassign From Team**

This Action Node remove an assignment from any team member automatically.

<figure><img src="../../../.gitbook/assets/image (504).png" alt="" width="191"><figcaption></figcaption></figure>

There is no settings for this Action Node. The contact will be automatically unassigned once it goes through this node.



## 5. Security Action Types:

### <img src="../../../.gitbook/assets/image (505).png" alt="" data-size="line">**Hide The File**

Secure sensitive files shared in the conversation. There is no settings for this Action Node.&#x20;

<figure><img src="../../../.gitbook/assets/image (506).png" alt="" width="175"><figcaption></figcaption></figure>



### <img src="../../../.gitbook/assets/image (507).png" alt="" data-size="line">**Mark The Text Messages As Per Regex**

Use regex patterns to identify and mark specific text messages for follow-up or categorization. There is no settings for this Action Node.&#x20;

<figure><img src="../../../.gitbook/assets/image (508).png" alt="" width="238"><figcaption></figcaption></figure>



## 6. Technical Action Types:

### <img src="../../../.gitbook/assets/image (509).png" alt="" data-size="line">**Call REST API**&#x20;

Integrate with external systems by calling REST APIs. Likewise sending information to the Rest API using the Push To CRM action type, you can also call/add the API of a 3rd party software or platform when needed using the automation for the particular Trigger.

<figure><img src="../../../.gitbook/assets/image (510).png" alt="" width="563"><figcaption></figcaption></figure>

According to your requirements and the platform's compatibility, add the REST API details. For instance,

* Type for URL as POST, GET, PUT, and DELETE.
* Input Header Key(s) and Value(s).
* Select Data Type as URL Encoded, JSON, or FORM.
* Then, add the JSON Data using the parameter fields, and once done, click **Add**.



### <img src="../../../.gitbook/assets/image (511).png" alt="" data-size="line">**Eval**

Execute custom scripts or code snippets for advanced processing.

<figure><img src="../../../.gitbook/assets/image (512).png" alt="" width="563"><figcaption></figcaption></figure>



## 7. Tagging Action Types:

### <img src="../../../.gitbook/assets/image (514).png" alt="" data-size="line">**Add Tags**

To automatically assign tags to the contact, you can utilize this particular Action Node. Click on the Tags field and simply select the existing tags from the drop down or define new ones and then click **Add**.

<figure><img src="../../../.gitbook/assets/image (513).png" alt="" width="563"><figcaption></figcaption></figure>

You can add multiple tags as needed.&#x20;

{% hint style="info" %}
This method will add new tags to the contact's existing ones without removing any.
{% endhint %}



### <img src="../../../.gitbook/assets/image (515).png" alt="" data-size="line">**Remove Tags**

Create an automation step to remove tags from the contact. Click on the Tags field and simply select the existing tag(s) you want to remove and click **Add**.

<figure><img src="../../../.gitbook/assets/image (516).png" alt="" width="563"><figcaption></figcaption></figure>



## 8. Whatsapp Chat Commerce Action Types:

### <img src="../../../.gitbook/assets/image (517).png" alt="" data-size="line">**Send Cart Confirmation Message**

Send messages to confirm cart contents and orders automatically.

<figure><img src="../../../.gitbook/assets/image (518).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
This is useful when you receive a Catalog Order from contact.
{% endhint %}



### <img src="../../../.gitbook/assets/image (519).png" alt="" data-size="line">**Send WhatsApp Notification**

Send a WhatsApp message to specific contact number(s) of your choice when the workflow reaches this action node.

<figure><img src="../../../.gitbook/assets/image (520).png" alt="" width="563"><figcaption></figcaption></figure>

You have to define the Phone Number, then select the template message to sent over.&#x20;

{% hint style="warning" %}
WhatsApp Message Template is chargeable based on the category. Refer to the WhatsApp API Conversation-Based Pricing
{% endhint %}

