# Events

An event in the Automation Workflows allows you to set different conditions to run automated actions.

<figure><img src="../../../.gitbook/assets/image (220).png" alt="" width="563"><figcaption><p>Default Automation Workflow Events Options</p></figcaption></figure>

{% hint style="info" %}
If you have integrated with marketplace, you will see more options here.&#x20;
{% endhint %}



## Event Types <a href="#trigger-types" id="trigger-types"></a>

Using Event, you can activate an automated action(s) based on the conditions fulfilled. It's highly useful to serve your customers in a timely manner and perform different actions when you're away from the platform. Or when you want to handle fewer tasks.

At Seampify, you can utilise these types of Automation Workflow Triggers:

* [New Outgoing Message ](events.md#new-outgoing-message)
* [New Incoming Message ](events.md#new-incoming-message)
* [User Lands on Bot (Welcome Event) ](events.md#user-lands-on-bot-welcome-event)
* [New Incoming Message From New Contact ](events.md#new-incoming-message-from-new-contact)
* [Conversation Closed ](events.md#conversation-closed)
* [When A Tag is Added ](events.md#when-a-tag-is-added)
* [When A Tag is Removed ](events.md#when-a-tag-is-removed)
* [Webhook Received ](events.md#webhook-received)

Each Event has a different set of conditions. Let's dive into each Event types and their respective available Trigger Conditions.



### New Outgoing Message

Automation is triggered when you or your teammate send a message to the contact using Chat.

<figure><img src="../../../.gitbook/assets/image (454).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for New Outgoing Message Event</p></figcaption></figure>



### New Incoming Message&#x20;

This is most commonly used. Automation is triggered when you receive a message on the selected Channel.

<figure><img src="../../../.gitbook/assets/image (455).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for New Incoming Message Event</p></figcaption></figure>



### User Lands on Bot (Welcome Event)&#x20;

Automation is triggered when a contact start a chat with your business.

<figure><img src="../../../.gitbook/assets/image (456).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for User Lands on Bot (Welcome Event) </p></figcaption></figure>



### New Incoming Message From New Contact&#x20;

Automation is triggered when you receive a message from a new contact for the first time.

<figure><img src="../../../.gitbook/assets/image (457).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for New Incoming Message From New Contact Event</p></figcaption></figure>



### **Conversation Closed**&#x20;

Automation is triggered when you or your teammate changes the conversation status to "Closed."

<figure><img src="../../../.gitbook/assets/image (458).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for <strong>Conversation Closed</strong> Event</p></figcaption></figure>



### When A Tag is Added&#x20;

Automation is triggered when you add a tag to a contact.

<figure><img src="../../../.gitbook/assets/image (459).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for When A Tag is Added Event</p></figcaption></figure>



### When A Tag is Removed&#x20;

Automation is triggered when you remove a tag from a contact.

<figure><img src="../../../.gitbook/assets/image (459).png" alt="" width="563"><figcaption><p>Trigger Conditions Options for When A Tag is Removed Event</p></figcaption></figure>



### Webhook Received&#x20;

Automation is triggered when a webhook is received on the selected channel. Once this event is chosen, a Webhook URL will be generated and you will need to configure using the webhook URL first.

<figure><img src="../../../.gitbook/assets/image (460).png" alt=""><figcaption></figcaption></figure>

### To configure Webhook URL:

{% stepper %}
{% step %}
### Sent some sample data to the webhook URL

Seampify receives data in JSON format, it is mandatory to have the phone number in order to send a message to that number, For example:

```postman_json
{
    "name":"Contact Name",
    "phone_number":"+60123456789"
}
```
{% endstep %}

{% step %}
### Map date to contact attributes

Once the webhook URL have receives the data, you will see the Map Data To Contact Attributes window. Here, you will need to map your data to the respective Contact Field in your Seampify account.

<figure><img src="../../../.gitbook/assets/image (461).png" alt=""><figcaption></figcaption></figure>

Left is the available Contact Field in your Seampify account. You may also create a new field from here if you couldn't find your desire Contact Field.

<figure><img src="../../../.gitbook/assets/image (462).png" alt="" width="299"><figcaption></figcaption></figure>

Right is the received data from your source to the Webhook URL. Click on the drop down menu to choose which data you wish to mapped.
{% endstep %}

{% step %}
### Click Map

Once data has been mapped, click on <img src="../../../.gitbook/assets/image (463).png" alt="" data-size="line"> button to save it. Then, you may proceed to [build your automation workflow](./#step-2-building-a-workflow) accordingly.



If you wish to edit the mapped data, click on the Map Data button on top right and it will open the Map Data To Contact Attributes window:

<figure><img src="../../../.gitbook/assets/image (464).png" alt="" width="495"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}
