---
description: Receiving Data into Seampify
---

# Seampify Webhook

Webhooks allow external systems to push data into Seampify automatically.

If an API is the _bridge_ that connects two systems, then a **webhook is like a custom “door” that you open specifically for receiving information**. Whenever your external system sends data to this door, Seampify receives it immediately and triggers the workflow you’ve configured.

Webhooks are commonly used for:

* Capturing leads from websites or ads
* Syncing booking appointments
* Logging game participants
* Creating automated WhatsApp messages
* Updating customer information
* Triggering chatbot flows



## **How it works**

Seampify is able to **receive incoming data in JSON format**, making it compatible with almost all modern systems.

### **1. Webhook Endpoint (Dynamic URL)**

Firstly, you will need a webhook endpoint to receive the data you intend to send to Seampify. Kindly contact the Seampify team to generate your **unique dynamic webhook URL** and to configure the correct attribute mappings and workflow actions that should run after the data is received.

Example format:

```
https://api.seampify.com/api/webhooks/dynamic-webhook/<unique-id>
```

Requests sent to this endpoint will be processed by the automation or workflow configured in Seampify.

### **2. Sending data over to Seampify**

Once the webhook endpoint is generated, your external system sends data to that URL using a standard HTTP POST request. Seampify receives the JSON payload and triggers the automation or workflow you’ve configured.

#### **Example JSON Payload**

* HTTP Method: `POST`
* Content-Type: `application/json`

```json
{
  "name": "John Doe",
  "phone": "+601112223333",
  "email": "john@example.com",
  "source": "Website Form"
}
```

{% hint style="warning" %}
Seampify can send WhatsApp messages worldwide. Please ensure that all phone numbers include the full country code with a “+” prefix. It is also recommended to include the customer’s name to ensure proper contact mapping in your Seampify database.
{% endhint %}

Seampify will respond with a JSON success message.

```json
{
  "status": "success",
  "message": "Payload received",
  "timestamp": "2025-12-04T10:32:55Z"
}
```

#### **Common HTTP Response Codes**

| Code    | Meaning                                                |
| ------- | ------------------------------------------------------ |
| **200** | Successfully processed                                 |
| **400** | Invalid request body                                   |
| **401** | Unauthorized (rare; only if access restrictions apply) |
| **500** | Server error (retry recommended)                       |

Once Seampify successfully processes the data, the assigned automation will be triggered. Examples include:

* Sending WhatsApp messages
* Inserting data into a Google Sheet
* Assigning a tag or label
* Logging to internal databases
* Updating contact attributes
* Triggering sequences or chatbot flows



## **Key Benefits of Seampify Webhooks**

* Real-time data capture
* No manual input needed
* Works with any platform that can send JSON
* Perfect for CRM sync and chatbot automation



## **Summary**

Seampify Webhooks provide an efficient way for external systems to send structured data to Seampify in real time. This enables businesses to automate WhatsApp communication, update customer records, log events, and drive workflows based on external triggers.



## **Testing the Seampify Webhook**

If you would like to test how Seampify Webhooks work, please follow the steps below:

{% stepper %}
{% step %}
### Send a WhatsApp Message

Send a message to: **+6019-989-3913**

This is required because the demo webhook operates within WhatsApp’s 24-hour Customer Service window. Sending a message first activates the chat session so Seampify can reply with the test message. \
\
You may also click the below to send us a message [https://wa.link/d3qv6t](https://wa.link/d3qv6t)
{% endstep %}

{% step %}
### **POST Your Test Data**

After initiating the chat, you may POST data to the demo webhook using the details provided below:&#x20;

**Request**

| Method | URL                                                                            |
| ------ | ------------------------------------------------------------------------------ |
| POST   | https://api.seampify.com/api/webhooks/dynamic-webhook/69311c11c89cf658f1c6b15b |

**Parameters**

| Key           | Value  | Description                                                                 |
| ------------- | ------ | --------------------------------------------------------------------------- |
| full\_name    | string | <p>(Required)<br>Contact’s Full Name</p>                                    |
| phone\_number | string | <p>(Required)<br>Contact’s Phone Number<br>{For example: +601123456789}</p> |
| email         | string | Contact’s Email Address (Optional)                                          |
| first\_name   | string | Contact’s First Name (Optional)                                             |
| last\_name    | string | Contact’s Last Name (Optional)                                              |
| test\_data    | string | <p>(Required)<br>Any testing information.</p>                               |

Example Curl Request/ payload:

| <p>curl --location 'https://api.seampify.com/api/webhooks/dynamic-webhook/69311c11c89cf658f1c6b15b'<br>--header 'Content-Type: application/json'<br>--header 'Cookie: AWSALB=rdmNFUJRDWsPI0EXr+GKRMd2iT0Vji5gH657hMhmx+EZ9X4LoyBT0hnQdeAf7RuA3xjYPz6leDf/3LPD7/39hjvINUEEq+Mn+eC3eJn+YyBRKyFYyAAK8oL128bM; AWSALBCORS=rdmNFUJRDWsPI0EXr+GKRMd2iT0Vji5gH657hMhmx+EZ9X4LoyBT0hnQdeAf7RuA3xjYPz6leDf/3LPD7/39hjvINUEEq+Mn+eC3eJn+YyBRKyFYyAAK8oL128bM'<br>--data-raw '{<br>"full_name": "Testing Name",<br>"phone_number": "+60123456789",<br>"email": "test@test.com",<br>"first_name": "Testing",<br>"last_name": "Name",<br>"test_data": "example info"<br>}'</p> |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |


{% endstep %}

{% step %}
### Receive the test message

Once your data is sucessfully posted over, Seampify will trigger our automation and send you the test message, example below:\
\
Hi there,\
\
Thanks for testing Seampify's Webhook function. Below is your posted data to us:\
\
&#x20;Full Name: Testing Name\
&#x20;Email: test@test.com\
&#x20;Test Data: example info\
\
Thanks for your testing again.
{% endstep %}
{% endstepper %}

#### Notes

* This webhook is for **testing purposes only**. Seampify team will provide you with the API document for actual use case.
