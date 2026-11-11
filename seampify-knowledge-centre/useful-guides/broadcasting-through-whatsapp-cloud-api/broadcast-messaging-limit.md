# Broadcast Messaging Limit

## Understanding Messaging Limit

Messaging limits are the maximum number of [business-initiated conversations](../conversation-through-whatsapp-cloud-api/understanding-whatsapp-message-template/) (conversations opened as a result of sending a marketing, utility, or authentication template to a WhatsApp user) a business phone number can open in a 24-hour moving period.

<figure><img src="../../.gitbook/assets/image (884).png" alt=""><figcaption><p>Messaging Limit Overview</p></figcaption></figure>

* **Sandbox Tier:** Right after signing up to Seampify, you can send message templates to up to 250 unique customers in a rolling 24-hour period without completing Business Verification.
* Tier 1: Allows your business to send **1k business-initiated conversations** **(2k unique customers)** in a rolling 24-hour period.
* Tier 2: Allows your business to send **10k business-initiated conversations** **(10k unique customers)** in a rolling 24-hour period.
* Tier 3: Allows your business to send **100k business-initiated conversations** **(100k unique customers)** in a rolling 24-hour period.
* Tier 4: Allows your business to send **unlimited business-initiated conversations**

{% hint style="success" %}
In any of the above tiers, businesses can reply to **unlimited user-initiated conversations**
{% endhint %}



## Increasing Messaging Limits <a href="#increasing_messaging_limits" id="increasing_messaging_limits"></a>

Business phone numbers are initially limited to 250 business-initiated conversations in a 24-hour moving period, but this limit can be increased.

{% hint style="warning" %}
Messaging limits are **not automatically increased**. Meta will analyze the messaging quality and activity to determine whether an increase is warranted.
{% endhint %}

* To upgrade out of Sandbox Tier, you need to send messages to 1,000+ unique contacts within a rolling 30-day period or verify your Meta Business Verification anytime.
* Once a business is in Tier 1, the business’s phone number will be upgraded to the next tier if:
  * your phone number status is **Connected**
  * your phone number quality rating is  is **Medium** or **High**&#x20;
  * in the last 7 days you have initiated X or more conversations with unique customers, where X is your current messaging limit divided by 2

If your business phone number meets all conditions above, the messaging limit will increase by one level, 24 hours later.



Here's an example of messaging limit increased from Tier 1 (2K) to Tier 2 (10K) in 2 days:

|                                                        | Day 1   | Day 2 | Day 3 | Day 4 |
| ------------------------------------------------------ | ------- | ----- | ----- | ----- |
| Business-initiated conversations opened                | 1,000   | 1,000 |       |       |
| Business-initiated conversations opened in last 7 days | 1,000\* | 2,000 |       |       |
| Messaging limit                                        | 2K      | 10K   |       |       |

\* If the 2,000th conversation is opened at 1pm (for example), the messaging limit is increased at 7pm on the same day (i.e. 6 hours later).



Here's another example of messaging limit increased from Tier 1 (2K) to Tier 2 (10K) in 4 days:

|                                                        | Day 1 | Day 2 | Day 3 | Day 4 |
| ------------------------------------------------------ | ----- | ----- | ----- | ----- |
| Business-initiated conversations opened                | 500   | 500   | 400   | 600   |
| Business-initiated conversations opened in last 7 days | 200   | 500   | 800\* | 500   |
| Messaging limit                                        | 2K    | 2K    | 2K    | 10K   |

\* If the 2,000th conversation is initiated at 3pm (for example), the messaging limit is increased at 9pm the same day (i.e. 6 hours later).&#x20;



## Checking Your Limit <a href="#checking-your-limit" id="checking-your-limit"></a>

Before your business phone number's messaging limit has been increased to 1K business-initiated conversations, the [**WhatsApp Manager**](https://business.facebook.com/wa/manage/home/) > **Overview** > **Limits** panel displays helpful information about what you can do to increase your limit.

<figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

After your business phone number's messaging limit has been increased, the [**WhatsApp Manager**](https://business.facebook.com/wa/manage/home/) > **Account tools** > **Phone Numbers > Insights** panel will display your business phone number's new limit, including new limits that have been increased as a result of [automatic scaling](https://developers.facebook.com/docs/whatsapp/messaging-limits#automatic-scaling).

<figure><img src="../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

Click on the number to open the Insights panel. Here, you can view the requirements to increase to the next messaging tier.

<figure><img src="../../.gitbook/assets/image (885).png" alt=""><figcaption></figcaption></figure>
