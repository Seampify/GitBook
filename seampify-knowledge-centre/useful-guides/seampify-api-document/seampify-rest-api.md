---
description: Sending Data Out From Seampify
---

# Seampify REST API

Unlike webhooks (which allow external systems to send data into Seampify), Seampify also supports sending data **out** to external systems using REST API calls.

This capability allows Seampify to integrate with a wide range of platforms, including:

* External CRMs (HubSpot, Zoho, Salesforce, etc.)
* Property management or automotive systems
* Loyalty or membership platforms
* ERP / POS systems
* Custom reporting dashboards
* Booking or reservation engines

***

## **Activation & Setup**

To enable REST API integration in your Seampify account, please contact **Seampify Support** and provide your system’s API documentation or endpoint specifications.

Seampify’s technical team will perform the setup and ensure all data is transmitted securely and successfully to your desired system.

***

## **How Seampify Sends Data Out**

Seampify uses the **“Call REST API”** function to post data to external endpoints.

#### **Supported HTTP Methods**

* `POST`
* `GET`
* `PUT`
* `PATCH`
* `DELETE`

#### **Supported Payload Formats**

* JSON body
* Query parameters
* Custom headers
* Dynamic variables from Seampify attributes
  * Example: `{phone_number}`, `{name}`, `{date}`

Dynamic variables are automatically replaced with actual customer or workflow values before the request is sent.

### **Example: Seampify Sending Data to an External System**

#### **Request**

```
POST https://partner-system.com/api/receiveData
Content-Type: application/json
Authorization: Bearer <token>
```

#### **Body**

```json
{
  "id": "{event_id}",
  "name": "{full_name}",
  "phone": "{phone_number}",
  "action": "booking_confirmed",
  "timestamp": "{timestamp}"
}
```

Variables inside `{ }` refer to the custom attributes or automation fields stored within your Seampify account. During execution, Seampify automatically replaces them with real data.

***

### **Example Response**

```json
{
  "received": true,
  "status": "ok"
}
```



## **Typical Use Cases**

* Send booking confirmations to Google Sheets or Google Calendar
* Push lucky draw results into a rewards database
* Sync renewal reminders with CRM systems
* Update customer status in ERP / POS systems
* Send order or payment details to an external platform

