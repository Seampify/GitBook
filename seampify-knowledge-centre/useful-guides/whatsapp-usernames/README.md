---
description: >-
  WhatsApp is introducing usernames—an optional feature that lets your business
  claim a unique handle (e.g., @Seampify) to help customers easily connect with
  you.
---

# WhatsApp Usernames

## Overview

WhatsApp is introducing **Usernames**, an optional feature that allows businesses and WhatsApp users to connect using a unique username instead of relying only on a phone number.

For businesses, a **WhatsApp Business Username** such as `@Seampify` gives customers an easier way to find and connect with your business.

Customers can also use a **WhatsApp Username** to contact businesses without necessarily sharing their phone number.

When this happens, Meta may provide your business with a **Business-Scoped User ID (BSUID)** instead of the customer's phone number.

> **In simple terms:** Your business can have a username, and your customers can also have usernames. Business usernames help customers find your business, while customer usernames can allow customers to interact with your business without revealing their phone number.

***

## Business Username vs Customer Username

There are two different types of WhatsApp usernames.

### Business Username

A **Business Username** belongs to your business and helps customers find and identify your WhatsApp Business account.

Example:

`@Seampify`

A Business Username:

* Is unique
* Helps customers discover your business
* Is associated with your WhatsApp Business phone number
* Does not replace your WhatsApp Business phone number
* Is optional and subject to Meta's eligibility and rollout requirements

### Customer Username

A **Customer Username** belongs to an individual WhatsApp user.

Customers can use their username to interact with businesses without necessarily sharing their phone number.

When a customer does this, Meta may provide your business with a **BSUID instead of the customer's phone number**.

***

## What is BSUID?

**BSUID stands for Business-Scoped User ID.**

When a customer contacts your business while their phone number is not available to the business, Meta may provide a BSUID to identify that customer.

Example:

`US.13491208655302741918`

The BSUID is generated and managed by Meta. Your business does not need to manually create one.

### Why does BSUID matter?

Previously, a customer's phone number was commonly used to identify a WhatsApp contact.

With WhatsApp Usernames, a customer may now be identified using:

**Phone Number OR BSUID**

This means a customer can exist in your CRM or messaging platform even when their phone number is not available.

***

## What Changes for Your Seampify Account?

For most businesses, no manual action is required to receive BSUIDs.

When a customer interacts with your Seampify WhatsApp account without sharing their phone number, Meta may provide a BSUID instead.

For example:

#### Previously

Customer → WhatsApp → Phone Number → Seampify Contact

#### With WhatsApp Username Privacy

Customer → WhatsApp → BSUID → Seampify Contact

The customer can still communicate with your business even when their phone number is unavailable.

***

## Can a Contact Exist Without a Phone Number?

**Yes.**

With WhatsApp Usernames, a customer may exist in Seampify with a BSUID but without a phone number.

The contact can still be used for supported WhatsApp conversations, chatbots and automation.

Businesses should therefore avoid assuming that every WhatsApp contact will always have a phone number.

***

## What Happens to Existing Contacts?

If businesses already has a customer's phone number, the phone number does not simply disappear because the customer starts using a WhatsApp Username.

Existing customer records can continue to contain the phone number that was previously available.

Customers who do not use username privacy can also continue to be identified through their phone number as usual.

***

## What Can I Do With a BSUID Contact?

A BSUID can be used to identify and communicate with a customer when their phone number is unavailable.

Depending on the applicable WhatsApp Business Platform capabilities and messaging rules, your business can continue to:

* Communicate with the customer
* Maintain the conversation history
* Trigger supported chatbot flows
* Trigger supported automation
* Manage the contact in your messaging platform

However, some use cases still require a phone number.

***

## Important: OTP and Authentication

WhatsApp authentication and OTP use cases require a **phone number**.

If your business uses WhatsApp for:

* OTP
* Account verification
* Authentication
* Other phone-number-dependent processes

you should have a flow to request the customer's phone number when it is not available.

> **BSUID should not be treated as a replacement for a phone number for every use case.**

***

## How Can I Collect the Customer's Phone Number?

If your business genuinely needs the customer's phone number, you can ask the customer to share it during the WhatsApp conversation.

For example:

> "Please share your phone number so we can verify your account and send your booking confirmation."

When requesting a phone number, we recommend clearly explaining why it is needed.

Depending on your use case, WhatsApp's supported contact-sharing and interactive features can be used to collect the customer's phone number.

***

## What Happens If I Have Multiple WhatsApp Numbers?

Businesses may have multiple WhatsApp Business Accounts and phone numbers.

BSUID is **business-scoped**, so its behaviour depends on how your WhatsApp Business Accounts are structured under Meta Business Portfolios.

#### Multiple WABAs Under the Same Business Portfolio

If multiple WhatsApp Business Accounts are under the same Business Portfolio, Meta can use the same business-scoped customer identifier to recognise the same customer across those accounts.

For example:

| WhatsApp Account | Customer | BSUID         |
| ---------------- | -------- | ------------- |
| Sales            | John     | `US.12345...` |
| Customer Service | John     | `US.12345...` |
| Marketing        | John     | `US.12345...` |

This allows businesses with multiple WhatsApp numbers under the same business structure to maintain a more consistent customer identity.

#### WABAs Under Different Business Portfolios

If your WhatsApp Business Accounts are under different Business Portfolios, the customer may have a different BSUID in each business context.

For eligible business structures operating across multiple Business Portfolios, Meta also provides **Parent BSUID** capabilities.

> **Parent BSUID is mainly relevant to businesses operating across multiple Business Portfolios. Most businesses with WABAs under a single Business Portfolio do not need to take additional action.**

***

## Frequently Asked Questions

<details>

<summary>Does a Business Username replace my WhatsApp phone number?</summary>

No.

A Business Username is an additional way for customers to find and connect with your business. Your WhatsApp Business phone number remains part of your WhatsApp Business Platform account.

</details>

<details>

<summary>Does every customer have a BSUID?</summary>

Businesses should be prepared to support BSUID because customers may choose to use username privacy.

Customers who do not use username privacy can continue to be identified through their phone number.

</details>

<details>

<summary>Can a customer exist in Seampify without a phone number?</summary>

Yes.

A customer may be created or identified using a BSUID when their phone number is unavailable.

</details>

<details>

<summary>Can I send WhatsApp messages to a BSUID?</summary>

BSUID can be used to identify a customer when their phone number is unavailable, subject to the applicable WhatsApp Business Platform capabilities and messaging rules.

</details>

<details>

<summary>Can I send OTP using BSUID?</summary>

No. WhatsApp authentication and OTP use cases require a phone number.

</details>

<details>

<summary>Can I search for a customer using their WhatsApp Username?</summary>

A WhatsApp Username should not be treated as a customer-search identifier.

Businesses generally obtain the relevant customer identifier when the customer interacts with the business.

</details>

{% hint style="info" %}
For the latest eligibility requirements, rollout information and technical documentation, please refer to Meta's official WhatsApp Business Platform documentation: [Username FAQs](https://faq.whatsapp.com/1594052115408959/?helpref=hc_fnav)
{% endhint %}

