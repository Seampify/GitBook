# All Meta Pricing You Need to Know

Understand how Meta charges for WhatsApp Business Platform messages, including marketing templates, utility messages, authentication messages, customer service replies, and WhatsApp calls.

When using Seampify to communicate with customers through the WhatsApp Business API, certain messaging activities may incur charges from Meta.

This guide explains how these charges work, when messages are free, and how to estimate your messaging costs.

{% hint style="info" %}
**Last updated: 22 October 2026**

**Important:** The pricing below refers to Meta's WhatsApp Business Platform charges, not Seampify's subscription or platform fees. Meta may revise its rates and billing policies. Always refer to the [official Meta pricing page](https://whatsappbusiness.com/products/platform-pricing/) for the latest rates.
{% endhint %}

### 1. How Does WhatsApp Business API Pricing Work?

Meta uses a **per-message pricing model**, meaning businesses are charged according to the type and number of messages successfully delivered to customers.

Your charges depend on three main factors:

1. **Message category:** Whether the message is marketing, utility, authentication, or service.
2. **Recipient's country:** Rates are based on the customer's WhatsApp phone number country code.
3. **Number of delivered messages:** Meta charges based on successful message delivery, not merely when a message is sent.

For example, a message delivered to a Malaysian number (+60) follows Malaysia's pricing, while a message delivered to a Singapore number (+65) follows Singapore's pricing.

This applies regardless of where your business is located.

\[Image]

### 2. WhatsApp Message Categories

Meta classifies WhatsApp Business Platform messages into four categories.

| Category       | Purpose                                           | Example                              |
| -------------- | ------------------------------------------------- | ------------------------------------ |
| Marketing      | Promotions, offers, announcements, and engagement | "Enjoy 20% off your next purchase!"  |
| Utility        | Transactional and account-related updates         | "Your order #1234 has been shipped." |
| Authentication | Identity verification through one-time passcodes  | "Your verification code is 482913."  |
| Service        | Non-template replies to customer enquiries        | "Hi! How can we help you today?"     |

Each category has different pricing rules.

#### Marketing Messages

Marketing messages are used to promote products, services, campaigns, or offers.

Common examples include promotional broadcasts, product launches, seasonal offers, customer re-engagement campaigns, and promotional reminders.

Marketing messages generally require an approved WhatsApp message template and appropriate customer opt-in.

**Marketing template messages are charged per delivered message**, unless a qualifying free-entry-point window applies.

#### Utility Messages

Utility messages provide important information relating to a customer's existing transaction, account, or request.

Examples include order confirmations, delivery notifications, appointment reminders, and payment receipts.

Utility messages must not contain unrelated promotional content.

From 1 October 2026, utility templates are generally chargeable even when sent within an open 24-hour customer service window, except when a qualifying free-entry-point benefit applies.

#### Authentication Messages

Authentication messages are used to verify a customer's identity, typically through one-time passwords (OTPs).

These messages use approved authentication templates and are charged per delivered message.

#### Service Messages

Service messages are non-template replies sent when a customer has initiated a conversation and the 24-hour customer service window is open.

These can include replies sent by your team through Seampify Inbox or by an automated chatbot or AI agent.

**From 1 October 2026, each WhatsApp business phone number receives 1,000 free delivered service messages per month.** Additional service messages are charged individually.

We explain this further in Section 4.

### 3. WhatsApp Business API Pricing for Singapore and Malaysia

The following are Meta's standard list rates for customers with Singapore (+65) and Malaysia (+60) phone numbers, based on rate cards applicable from 1 October 2026.

| Message Category                      | Singapore (SGD) | Malaysia (MYR) |
| ------------------------------------- | --------------- | -------------- |
| Marketing                             | S$0.0937        | RM0.3467       |
| Utility                               | S$0.0205        | RM0.0564       |
| Authentication                        | S$0.0205        | RM0.0564       |
| Service, after monthly free allowance | S$0.0205        | RM0.0564       |

**Please note:**

* Rates are shown per successfully delivered message.
* Prices exclude applicable taxes, Seampify platform fees, and other potential charges.
* Utility and authentication messages may qualify for volume-based discounts.
* Service messages have a monthly free allowance but no volume-based discount.
* Actual billing depends on your WhatsApp Business Account's billing currency. An account billed in another currency may show different rate-card amounts.

You can also view Meta's latest rate cards on its [official WhatsApp pricing page](https://whatsappbusiness.com/products/platform-pricing/).

### 4. Understanding Service Message Pricing (Effective 1 October 2026)

Previously, businesses could send free-form customer service replies during an open 24-hour customer service window without Meta messaging charges.

**This changed on 1 October 2026.**

Meta now provides a free monthly allowance of 1,000 delivered service messages per WhatsApp business phone number.

Once the allowance is used, additional service messages are charged at the applicable country rate.

#### How the Free Allowance Works

Suppose your business has one connected WhatsApp number.

During October:

* Your first 1,000 delivered service messages are free.
* Your 1,001st service message is chargeable.
* Every subsequent delivered service message is charged at the applicable service rate.
* The allowance resets at the beginning of the next month.
* Unused free messages do not carry forward.

The allowance applies individually to each WhatsApp business phone number.

#### Example: Malaysia

Your business sends 2,500 delivered service messages to Malaysian customers during October.

| Description                      | Messages |
| -------------------------------- | -------- |
| Total delivered service messages | 2,500    |
| Free monthly allowance           | 1,000    |
| Chargeable service messages      | 1,500    |

**Estimated Meta charges:**

1,500 × RM0.0564 = **RM84.60**

#### Example: Singapore

Your business sends 2,500 delivered service messages to Singaporean customers during October.

1,500 × S$0.0205 = **S$30.75**

These examples assume one business phone number, recipients in one country, standard service rates, and no other applicable exemptions.

#### Important: A Conversation Is Not the Same as a Message

If your customer sends one enquiry and your agent responds using five separate messages, Meta counts five delivered service messages.

The same principle applies to automated replies.

For example, an AI agent sending one answer in five separate message bubbles may incur five service-message charges after the free allowance is exhausted.

Businesses should therefore aim for clear, concise responses rather than unnecessarily splitting answers into multiple messages.

### 5. Understanding the 24-Hour Customer Service Window

When a customer messages your business, Meta opens a **24-hour customer service window**.

During this period, your business can reply using non-template messages.

Every new customer message resets the 24-hour window.

#### Example

A customer sends a WhatsApp message at 10:00 AM on Monday.

Your business may respond with non-template messages until 10:00 AM on Tuesday, provided the customer does not send another message.

If the customer replies again at 3:00 PM on Monday, the window is extended until 3:00 PM on Tuesday.

After the window closes, your business must use an approved WhatsApp message template to initiate further messaging.

**Important:** An open 24-hour window does not automatically mean all business replies are free. The service-message and template-message pricing rules still apply.

### 6. When Can WhatsApp Messages Be Free?

Although Meta generally charges per delivered message, some messaging scenarios remain free.

#### A. Customer-Initiated Messages

Messages sent by customers to your business are free.

For example, when a customer sends "Hi, is this product available?", your business is not charged for receiving that message.

Your business's replies follow the applicable service-message pricing rules.

#### B. First 1,000 Service Messages Each Month

Every connected WhatsApp business phone number receives 1,000 free delivered service messages per month.

This allowance applies to eligible non-template replies within the 24-hour customer service window.

#### C. Free-Entry-Point Conversations

When a customer contacts your business through a qualifying **Click-to-WhatsApp ad** or Facebook Page call-to-action button, Meta may open a free-entry-point window.

When the business responds within the required eligibility period, eligible messages can be sent without Meta messaging charges during a 72-hour free-entry-point window.

For example:

1. A customer clicks your Click-to-WhatsApp advertisement.
2. The customer sends your business a WhatsApp message.
3. Your business responds within the qualifying period.
4. Meta opens the free-entry-point window.
5. Eligible messages sent within this window are not charged.

Please note that advertising costs for Click-to-WhatsApp campaigns are separate from WhatsApp messaging fees.

### 7. WhatsApp Calling API Pricing

Seampify may support WhatsApp calling features for eligible connected business numbers.

WhatsApp Business Calling API pricing is separate from text-message pricing.

Call charges depend on factors such as the call direction, destination or country, and the applicable Meta calling rate.

Unlike message templates, calls may be charged based on billable call duration rather than the number of messages delivered.

Before enabling WhatsApp calling, review the applicable rates and feature availability for your business.

For current calling rates, please refer to Meta's official business messaging documentation.

### 8. How to Estimate Your Monthly WhatsApp Messaging Costs

You can estimate your Meta messaging expenses using the number of chargeable delivered messages in each category.

**Estimated messaging cost = Sum of (chargeable delivered messages × applicable message rate)**

#### Example: A Business Sending Messages to Malaysian Customers

Assume your business sends the following messages during one month:

| Message Type   | Monthly Messages         | Rate     | Estimated Cost |
| -------------- | ------------------------ | -------- | -------------- |
| Marketing      | 2,000                    | RM0.3467 | RM693.40       |
| Utility        | 1,000                    | RM0.0564 | RM56.40        |
| Authentication | 200                      | RM0.0564 | RM11.28        |
| Service        | 2,500 (1,500 chargeable) | RM0.0564 | RM84.60        |
| **Total**      |                          |          | **RM845.68**   |

This illustration assumes all chargeable messages are successfully delivered, no volume discounts apply, and there are no special exemptions.

Your actual billing may vary depending on message category, recipient location, volume tier, and any free-entry-point eligibility.

### 9. Meta Charges vs. Seampify Charges

It is important to understand that **Meta messaging charges and Seampify platform charges are separate**.

#### Meta Messaging Charges

These are charges determined by Meta for WhatsApp Business Platform usage, including billable template messages, service replies, and applicable WhatsApp calling activity.

#### Seampify Platform Charges

These relate to the Seampify services and features included in your selected plan.

Your Seampify subscription does not automatically mean that all Meta WhatsApp messaging charges are included.

For details about your Seampify subscription, included features, and any additional platform charges, refer to your Seampify quotation or contact our support team.

### 10. Frequently Asked Questions

#### Is WhatsApp Business API free?

The WhatsApp Business Platform does not charge a separate Meta licence fee for accessing its messaging API, but messaging usage can incur charges.

Some messages qualify for free allowances or special free-entry-point arrangements.

#### Do I get 1,000 free conversations per month?

No. From 1 October 2026, the relevant free allowance is **1,000 delivered service messages per business phone number per month**, not 1,000 conversations.

#### Will I be charged when a customer messages my business?

No. Messages received from customers are free. Charges may apply when your business responds.

#### Are messages sent by automation or AI agents free?

Not necessarily. Non-template replies sent by an automation or AI agent are generally subject to the same service-message rules as manually written replies.

#### Can I send marketing messages during the 24-hour customer service window for free?

Marketing templates are generally chargeable even when the customer service window is open, unless a qualifying free-entry-point window or another applicable exemption applies.

#### Does the 1,000-message allowance apply to marketing broadcasts?

No. The allowance applies to service messages, not marketing templates.

#### Are unsuccessful messages charged?

Meta generally charges when a message is successfully delivered, not merely when your business attempts to send it.

#### Why are Singapore and Malaysia message rates different?

Meta sets different rates for different recipient markets. A message to a Singapore number uses Singapore's rates, while a message to a Malaysian number uses Malaysia's rates.

#### Can Meta change these prices?

Yes. Meta may update its pricing, message category rules, discounts, and free-message allowances.

For the latest information, always refer to Meta's official pricing documentation.

***

Learn more for each conversations from the links below:

{% content-ref url="conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md" %}
[understanding-24-hour-customer-service-window.md](conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md)
{% endcontent-ref %}

{% content-ref url="conversation-through-whatsapp-cloud-api-1/understanding-whatsapp-message-template/" %}
[understanding-whatsapp-message-template](conversation-through-whatsapp-cloud-api-1/understanding-whatsapp-message-template/)
{% endcontent-ref %}

{% content-ref url="conversation-through-whatsapp-cloud-api-1/whatsapp-conversation-based-pricing/" %}
[whatsapp-conversation-based-pricing](conversation-through-whatsapp-cloud-api-1/whatsapp-conversation-based-pricing/)
{% endcontent-ref %}
