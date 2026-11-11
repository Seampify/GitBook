# Create a New Automation

## Step 1: Setup Automation Workflow

To create an automation workflow from scratch, click the **Add New Automation** button.

<figure><img src="../../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

This will open the Create Automation Workflow modal with the options as -

* Automation Name
* Channel / Service Integration (trigger dependent)
* [Trigger Event](events.md)

<figure><img src="../../../.gitbook/assets/image (218).png" alt=""><figcaption></figcaption></figure>

{% stepper %}
{% step %}
### Define a Name

In the Create Automation Workflow modal, first, you need to define a name for the automation.&#x20;
{% endstep %}

{% step %}
### Select Channel

Then, select a Channel from the available options.

<div align="left"><figure><img src="../../../.gitbook/assets/image (219).png" alt="" width="391"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Select Event

After selecting the Channel, you need to pick an Event to trigger the automation.&#x20;

<div align="left"><figure><img src="../../../.gitbook/assets/image (220).png" alt="" width="563"><figcaption></figcaption></figure></div>

If you have integrated with marketplace, you will see more options here. By default, you will see these options:

* **New Outgoing Message** - Automation is triggered when you or your teammate send a message to the contact using Chat.
* **New Incoming Message** - Automation is triggered when you receive a message on the selected Channel.
* **User Lands on Bot (Welcome Event)** - Automation is triggered when a contact start a chat with your business.
* **New Incoming Message From New Contact** - Automation is triggered when you receive a message from a new contact for the first time.
* **Conversation Closed** - Automation is triggered when you or your teammate changes the conversation status to "Closed."
* **When A Tag is Added** - Automation is triggered when you add a tag to a contact.
* **When A Tag is Removed** - Automation is triggered when you remove a tag from a contact.
* **Webhook Received** - Automation is triggered when a webhook is received on the selected channel.&#x20;

Each Event has a different set of conditions. Learn more about [Events](events.md) and [Trigger Conditions](trigger-conditions.md) in the next step.
{% endstep %}

{% step %}
### Click Create

Select <img src="../../../.gitbook/assets/image (221).png" alt="" data-size="line"> button once done.
{% endstep %}
{% endstepper %}



## Step 2: Building a Workflow

Once you have setup the Automation Workflow settings, you will goes to the Automation window. By default, each automation will have one Trigger node.

<figure><img src="../../../.gitbook/assets/image (222).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Click the <img src="../../../.gitbook/assets/image (223).png" alt="" data-size="line">  **pause button** to deactivate the automation while building it. This ensures the automation won’t accidentally trigger before it’s ready.
{% endhint %}

{% stepper %}
{% step %}
### Set Trigger Node

Double click on the Trigger node to open its settings on the right. Simply select the required Trigger Condition and update node.

<figure><img src="../../../.gitbook/assets/trigger.gif" alt=""><figcaption></figcaption></figure>

Based on your selected Event in step 1, you get the list of Trigger Conditions. [Learn more about list of Trigger Conditions for each event here](events.md#trigger-types).
{% endstep %}

{% step %}
### Add Steps

To add Workflow Steps, click the <img src="../../../.gitbook/assets/image (224).png" alt="" data-size="line"> **lighting button** to access Action types. This will open the Workflow Steps modal with all the step types. Simply select your desire Action nodes from the list and drag and drop to the workflow window.&#x20;

<div align="left"><figure><img src="../../../.gitbook/assets/action.gif" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
You may also right click on the window to access Action types on the left.
{% endhint %}

To learn how each step works and what's the best way to configure them, visit [Action Steps.](actions-steps.md)
{% endstep %}

{% step %}
### Setup Action Step

Double click on the Action nodes to open its settings on the right. Fill up the settings and click **Update Node** once done.

<figure><img src="../../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Connect Action Step

Connect the Action nodes by clicking on the <img src="../../../.gitbook/assets/image (226).png" alt="" data-size="line"> button on the right and dragging it to the green dot <img src="../../../.gitbook/assets/image (227).png" alt="" data-size="line"> on the left of the Action nodes.

<div align="left"><figure><img src="../../../.gitbook/assets/drag.gif" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Add More Action Step

To add more Action nodes, repeat the steps and choose the desire Action nodes from the list and drag and drop to the workflow window.&#x20;
{% endstep %}

{% step %}
### Click Save

Once your workflow is done, click on the <img src="../../../.gitbook/assets/image (228).png" alt="" data-size="line"> button.

{% hint style="info" %}
Remember to click the <img src="../../../.gitbook/assets/image (230).png" alt="" data-size="line"> button to activate the Automation.&#x20;

It is recommended to test your Automation before publishing. [Learn more here](testing-your-automation.md)
{% endhint %}
{% endstep %}
{% endstepper %}
