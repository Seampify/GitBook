---
description: >-
  This template helps businesses automate the post-order experience on WhatsApp,
  from sending cart confirmation to collecting payment using Stripe and handling
  follow-ups.
---

# Import Checkout Automation

## _📘 Guide: How to Use the Ecommerce Order Received Automation Template in Seampify (with Stripe)_

***

{% hint style="info" %}
This guide is for users **who do  have Stripe integrated**. If you do not have Stripe, please refer to the [without Stripe](import-checkout-automation.md#how-to-use-the-ecommerce-order-received-automation-template-in-seampify-without-stripe) version of the guide instead.
{% endhint %}

### ✅ Step 1: Load the Template

<figure><img src="../../.gitbook/assets/image (872).png" alt=""><figcaption></figcaption></figure>

1. **Go to the Automation > Import Automation Template > Ecommerce**
2. Choose "**Ecommerce Order Received**_"_
3. Click **“Preview”** to load it.&#x20;
4. Click Import

<figure><img src="../../.gitbook/assets/image (873).png" alt=""><figcaption></figcaption></figure>

5. Give your automation a name.
6. Choose your **WhatsApp Channel**.
7. Set the trigger to **New Incoming Message**.
8. Click **Save**.

<figure><img src="../../.gitbook/assets/image (874).png" alt=""><figcaption></figcaption></figure>

***

### ⚙️ Step 2: Configure the Trigger

* **Trigger Node:** `new_catalog_order_received`

<figure><img src="../../.gitbook/assets/image (875).png" alt=""><figcaption></figcaption></figure>

* This automatically starts the flow when someone places an order via your WhatsApp catalog.
* ✅ _No manual setup needed here — it’s already pre-configured._

***

### ✍️ Step 3: Edit Messages (Optional)

You can customize the messages in the following nodes:

**🛒 Cart Confirmation**

**Node:** _Send Cart Confirmation Message_

<figure><img src="../../.gitbook/assets/image (876).png" alt=""><figcaption></figcaption></figure>

*   You can edit message body:

    ```
    Thank you for your order. Here's your cart details:
    {cart_products}
    Total Order Value: *{cart_total}*
    Would you like to checkout?
    ```
* Can edit button Texts:
  * "Checkout"
  * "Maybe later"

***

### 💳 Step 4: Setup Stripe Payment

**Node:** _Stripe Send Payment Link_

<figure><img src="../../.gitbook/assets/image (877).png" alt=""><figcaption></figcaption></figure>

1. Make sure your Stripe account is connected in Seampify.
2. The payment link will automatically include the cart items.
3. You can optionally define:
   * Up to 5 extra items manually
   * Custom quantities & prices

✅ _No need to add any webhook — handled natively via Seampify + Stripe integration._

***

### ⏱️ Step 5: Customize Follow-up Timing

**Node:** _Delay Execution_

<figure><img src="../../.gitbook/assets/image (878).png" alt=""><figcaption></figcaption></figure>

* Currently set to **30 minutes** after Stripe link is sent.
* You can:
  * Increase for a softer approach (e.g., 1 hour).
  * Decrease if you're targeting quick conversions (e.g., 15 mins).

***

### 🔁 Step 6: Configure Reminder Behavior

<figure><img src="../../.gitbook/assets/image (879).png" alt=""><figcaption></figcaption></figure>

**You can edit the reminder Node:**

* If the user hasn’t completed payment, a reminder message will be sent:
  * “Oh no, we have not received a payment. Would you like to continue?”

**Can edit Buttons:**

* "Continue Checkout" → Resend Stripe link
* "Maybe later" → Gentle exit message

***

### 🧑‍💼 Step 7: Assign to Team Member

<figure><img src="../../.gitbook/assets/image (880).png" alt=""><figcaption></figcaption></figure>

* If the user does **not respond to the reminder**, the system sends a final fallback message and automatically assign to team member. You can set here to assign it to whom by choosing the options&#x20;
* **Click Save** once all editing is done and you may test your automation accordingly.

## _📘How to Use the Ecommerce Order Received Automation Template in Seampify (without Stripe)_

If you prefer to **send payment links manually** instead of using Stripe integration, follow the simple steps below to adjust the template accordingly:

### 🔧 Step 1: Remove the Stripe Payment Link Node

1. locate the node labeled:
   * **“Stripe Send Payment Link”**
2. **Click the node once** to select it.
3. Press the **`Backspace` or `Delete`** key on your keyboard to remove it.
4. Alternatively, you can **unlink** it:
   * Click the **small black dot** (<img src="../../.gitbook/assets/image (883).png" alt="" data-size="line">) on the edge of the connected line.
   * Then **drag it away** or click to break the connection.

<figure><img src="../../.gitbook/assets/image (882).png" alt=""><figcaption></figcaption></figure>

### 🔗 Step 2: Reconnect the Flow

1. Reconnect the nodes that were linked to the Stripe node to **continue the flow smoothly**.
2. For example:
   * After the **Cart Confirmation Message**, you can directly link to:
     * A **Reminder Node** (e.g., “Would you like to continue checkout?”), or
     * A **Delay Node**, then to the Reminder
   * If no response is received, connect to the **Fallback message** and **Assign to Team Member**.

📸 _Refer to the visual diagram below to follow the recommended linking path._

<figure><img src="../../.gitbook/assets/image (881).png" alt="" width="563"><figcaption></figcaption></figure>

#### 💡 Note:

* By removing the Stripe node, this template now becomes a **semi-manual flow**.
* You’ll **manually send the payment link** during live chat in Seampify Inbox after the customer confirms.
* This approach gives you **more control** over how and when you send payment links.
