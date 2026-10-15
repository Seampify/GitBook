---
description: >-
  If your automation is not working as expected, follow the steps below to
  resolve the issue.
---

# Why is My Automation Not Working?

## **1. Make Sure the Automation is Played**

* The first step is to ensure that the automation has been played.
* **Action**: Click the "Play" button to start the automation.

<figure><img src="../../.gitbook/assets/Screenshot 2025-01-23 142124.png" alt="" width="440"><figcaption></figcaption></figure>

* The automation won’t run unless it's activated manually.

***

## **2. Check the Trigger Node**

The trigger node is critical for determining when the system should perform automation.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/image (771).png" alt="" width="379"><figcaption></figcaption></figure></div>

Ensure it is configured based on the **condition you want to use** and apply it accordingly. Follow these steps to ensure the trigger node is set up correctly:

* **To perform automation triggered by ads**:
  * Ensure to use  `Custom Condition`

<figure><img src="../../.gitbook/assets/ScreenRecording2025-01-24162338-ezgif.com-video-to-gif-converter.gif" alt=""><figcaption></figcaption></figure>

*   **To automate actions triggered by button clicks:**

    * **Set the Callback ID for Buttons**

    <figure><img src="../../.gitbook/assets/image (774).png" alt=""><figcaption></figcaption></figure>

    * Ensure the callback ID in the button of template matches the callback ID in the automation.

    <figure><img src="../../.gitbook/assets/image (775).png" alt=""><figcaption></figcaption></figure>
* **Handle  First or After-24-Hour Messages**:
  * This trigger node will play automation when:
    1. There is a **new incoming message** from the customer for the first time.
    2. There is an **incoming message after the 24-hour chat window** has expired.

<figure><img src="../../.gitbook/assets/ScreenRecording2025-01-24164401-ezgif.com-video-to-gif-converter.gif" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="warning" %}
**Note**: Automation will not run if the first message is initiated by you. The system only works if the customer sends the first message.
{% endhint %}

*   **Ensure Keyword Matches**:

    * The **keyword exactly matches trigger node** will only perform automation when the system detects incoming messages that exactly match the specified keywords.

    <figure><img src="../../.gitbook/assets/image (777).png" alt=""><figcaption></figcaption></figure>
