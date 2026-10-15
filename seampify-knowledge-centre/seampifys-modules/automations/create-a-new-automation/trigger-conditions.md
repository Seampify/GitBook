# Trigger Conditions

Each Automation will have at least one Trigger Node for you to define the Trigger Condition(s).&#x20;

<figure><img src="../../../.gitbook/assets/image (435).png" alt=""><figcaption></figcaption></figure>

Trigger Condition(s) is the basis for an automated action(s) to run. There are multiple types of Conditions, which, if fulfilled, the Action(s) will be executed.&#x20;

{% hint style="warning" %}
The list of Trigger Condition options is based on the Event you have chosen in the previous step.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (433).png" alt=""><figcaption><p>List of Trigger Conditions</p></figcaption></figure>

You may add multiple Trigger Condition in each Trigger Node. To do this, click on the <img src="../../../.gitbook/assets/image (442).png" alt="" data-size="line"> button and it will open up another Trigger Condition field like this:

<figure><img src="../../../.gitbook/assets/image (443).png" alt=""><figcaption></figcaption></figure>

The Automation will only be triggered if both Trigger Conditions are met/ fulfilled.



## Trigger Condition Types

The are multiple types of Trigger Conditions you can use for the Automation Workflow at Seampify, which are:

### **Message text exactly matches**

This trigger condition is available when you select the _New Outgoing/Incoming Message_ Event. Under this condition, the message should exactly match any of the _**Text Keywords**_ to activate the trigger and run the action.

<figure><img src="../../../.gitbook/assets/image (436).png" alt=""><figcaption></figcaption></figure>

You may add multiple keywords and the automation will be triggered once any of the keyword inserted here is matched.

Enable **"Is Case Sensitive"** if you want the keyword to match exactly, including its case.



### **Message text includes any of keywords**

This trigger condition is available when you select the _New Outgoing/Incoming Message_. Under this condition, if the message includes one/any of the mentioned _**Text keywords**_, the trigger will be activated, and the action will run.

<figure><img src="../../../.gitbook/assets/image (437).png" alt=""><figcaption></figcaption></figure>

The entire message doesn't need to be precisely the same as the Text Keywords. Similarly, you may add multiple keywords and the automation will be triggered once any of the keyword inserted here is matched.

Enable **"Is Case Sensitive"** if you want the keyword to match exactly, including its case.



### Message text exclude any of keywords

This trigger condition is available when you select the _New Outgoing/Incoming Message_. Under this condition, the trigger will be activated to all message except if the message exclude one/any of the mentioned _**Text keywords**_, then the action will not run.

<figure><img src="../../../.gitbook/assets/image (438).png" alt=""><figcaption></figcaption></figure>

The entire message doesn't need to be precisely the same as the Text Keywords. Similarly, you may add multiple keywords here.

Enable **"Is Case Sensitive"** if you want the keyword to match exactly, including its case.



### List/Button Callback ID matches

Under this trigger condition, the automation will execute the action if the _New Outgoing/Incoming Message_ is an button type message and its List ID/Button Callback ID matches the **Callback ID**.

<figure><img src="../../../.gitbook/assets/image (439).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The Callback ID does not need to match the Button name exactly. It is used by the system to identify and match the keyword in the backend when the button is clicked.
{% endhint %}

You may add multiple Callback ID and the automation will be triggered once a button with its List ID/Button Callback ID matches to any of the one inserted here is clicked.

Enable **"Is Case Sensitive"** if you want the keyword to match exactly, including its case.



### Received outside business hours

Run an automation workflow action when the _New Incoming Message_ is received outside the business hours.

<figure><img src="../../../.gitbook/assets/image (440).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Set your business hours using the My Account settings.
{% endhint %}



### Received Inside Business Hours

Run an automation workflow action when the _New Incoming Message_ is received during the business hours.

<figure><img src="../../../.gitbook/assets/image (441).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Set your business hours using the My Account settings.
{% endhint %}



### New Catalog Order Received

If you've created Product Catalogs in the WhatsApp Store Settings, you can create automation based on them. It will trigger on _New Incoming Message_ when your contacts submit a catalog request after selecting products through the interactive message you sent.

<figure><img src="../../../.gitbook/assets/image (444).png" alt=""><figcaption></figcaption></figure>



### Very first message or message after 24hrs of last message

Run an automation workflow action that needs to be executed when the _New Incoming Message_ received is the Very First Message or the Message after 24hrs of the last message in the selected channel.

<figure><img src="../../../.gitbook/assets/image (445).png" alt=""><figcaption></figcaption></figure>



### All Messages / No Condition

This trigger condition is available when you select the _New Incoming Message, New Incoming Message From New Contact, Conversation Closed or Webhook Received_ Event. The automation will be triggered when any of the mentioned event occurs  <mark style="color:red;">without any other condition.</mark>

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>



### Custom Condition

This trigger condition is available when you select the _New Outgoing/Incoming Message or Webhook Received_ Event. For this condition to activate, once a new outgoing / incoming message or a webhook data received event occurs with a contact, the contact’s attribute must match the specified **Match String** to trigger the action.&#x20;

<figure><img src="../../../.gitbook/assets/image (449).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
This trigger condition is ideal for activating a specific action based on interactions from a particular **Click-To-WhatsApp Ad (CTWA)**.
{% endhint %}

#### Custom Condition for Click-To-WhatsApp Ad (CTWA)

If you're running Click-To-WhatsApp Ads (CTWA) on Facebook or Instagram and want to trigger specific automations for each ad, you can use **Custom Condition Trigger Nodes**.

The **Custom Conditions' Messaging Attributes** payload key offers three ways to define and trigger a specific automation:

1. **Referral Source ID**
   * Use this to trigger automations based on a specific ad's unique ID.
   * Ideal when you have multiple ads running simultaneously and need different automations for each ad.
2. **Referral Source Type**
   * Use this to trigger automations based on the type of source, such as a **post** or an **ad**.
   * Suitable when you want to trigger the same automation for all posts or all ads.
3. **Referral Source URL**
   * Use this to trigger automations based on a specific ad's URL.
   * Useful when managing multiple ads simultaneously and needing unique automations for different ads.

These options allow you to customize your workflows and optimize your ad-driven WhatsApp interactions effectively.

<figure><img src="../../../.gitbook/assets/image (163).png" alt=""><figcaption></figcaption></figure>

### File Type Matches

Run an automation workflow action when the _New Outgoing/Incoming Message_ is a file type, and its extension matches the one you specify (e.g., `.jpg`, `.png`, `.gif`, etc.).

<figure><img src="../../../.gitbook/assets/image (450).png" alt=""><figcaption></figcaption></figure>

You can add multiple extension in a Trigger Condition.



### Message Text Regex Matches

Run an automation workflow action when the _New Outgoing/Incoming Message_ matches the Regex you specify.

<figure><img src="../../../.gitbook/assets/image (451).png" alt=""><figcaption></figcaption></figure>



### Message Type

Run an automation workflow action when the _New Outgoing/Incoming Message_ matches the message type you chosen.

<figure><img src="../../../.gitbook/assets/image (452).png" alt=""><figcaption></figcaption></figure>



### Tag include any of keywords

This trigger condition is available when you select the _New Incoming Message From New Contact, Conversation Closed_, or _When A Tag is Added/Removed_ event. For this condition to activate, any of the selected events must occur, and the contact must have a tag that matches one of the tags specified in the trigger conditions to execute the action.

<figure><img src="../../../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

You may add more than one tags for each Trigger Conditions.
