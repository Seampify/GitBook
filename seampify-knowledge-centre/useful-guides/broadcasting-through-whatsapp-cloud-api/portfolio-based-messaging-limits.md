# Portfolio-based  Messaging Limits

**Starting October 7, 2025**, Meta is changing how messaging limits work. Instead of limits being tied to each phone number, they’ll now be applied at the **business portfolio level** and shared across all numbers in the portfolio.

Existing business portfolios will have their messaging limit set to the highest limit of any phone number within their portfolio (e.g. if a portfolio has a phone number with a limit of 100K and other phone numbers with lower limits, the portfolio's limit will be set to 100K).<br>

How does this work?

* **Shared Limits**: \
  All numbers under the same portfolio will use the same messaging limit.
* **Higher Inheritance**: \
  The portfolio will take on the **highest limit** among its numbers.\
  _&#x45;xample: If one number has 100K and another has 10K, the portfolio limit becomes 100K._



These changes will result in:

* **Faster access to higher limits**, with upgrades within 6 hours (compared to the current 24 hours) and immediate access to the portfolio's limits for newly registered numbers.
* **Greater flexibility**, allowing you to have as many phones as needed without requiring additional phones to access higher limits, since all phones share the portfolio's limit.
* **Reduced administrative burden and operational costs**, by minimizing the need for unnecessary phone numbers.



### Changes <a href="#changes" id="changes"></a>

|                                                          | Before Oct 7th, 2025                                                                                                                                                                                                                                                                                                           | Starting Oct 7th, 2025                                                                                                                                                                                                                                                                                                           |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Where are limits set?**                                | <p>On individual business phone numbers.</p><p></p><p>For example, phone number A could have a limit of 10K but phone number B could have a limit of 100K.</p>                                                                                                                                                                 | <p>On individual business portfolios.</p><p></p><p>For example, a portfolio with 2 phone numbers could have a 100K limit shared by both numbers.</p>                                                                                                                                                                             |
| **Starting limit for newly created business portfolios** | Not applicable                                                                                                                                                                                                                                                                                                                 | 250                                                                                                                                                                                                                                                                                                                              |
| **Starting limit for a newly registered number**         | 250                                                                                                                                                                                                                                                                                                                            | Shares the messaging limit set on the business portfolio.                                                                                                                                                                                                                                                                        |
| **Limit upon becoming eligible for automatic scaling**   | 1,000                                                                                                                                                                                                                                                                                                                          | 2,000                                                                                                                                                                                                                                                                                                                            |
| **Time to increase limit via automatic scaling**         | Limit increased 24 hours after meeting criteria.                                                                                                                                                                                                                                                                               | Limit increased 6 hours after meeting criteria.                                                                                                                                                                                                                                                                                  |
| **Phone number quality states**                          | <p>The <strong>Flagged</strong> <a href="https://www.facebook.com/business/help/896873687365001">phone number quality</a> state is possible.</p><p></p><p>If your business phone number quality rating has been set to <strong>Flagged</strong> for the last 7 days, we will decrease its limit by one level, immediately.</p> | <p>The <strong>Flagged</strong> <a href="https://www.facebook.com/business/help/896873687365001">phone number quality</a> state is no longer exists.</p><p></p><p>If your business phone number quality rating drops, its messaging limit will not be downgraded.</p>                                                            |
| **Automatic scaling criteria**                           | <ul><li>Your business phone number is connected</li><li>Your business phone number quality rating is <strong>Medium</strong> or <strong>High</strong>)</li><li>In the last 7 days, your business has utilized at least half of your current messaging limit</li></ul>                                                          | <ul><li>You are sending <a href="https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-messages#message-quality">high-quality messages</a> across all of your business phone numbers and templates.</li><li>In the last 7 days, your business has utilized at least half of your current messaging limit</li></ul> |

## Portfolio-based Messaging Limits in overall

<figure><img src="../../.gitbook/assets/image (884).png" alt=""><figcaption><p>Messaging Limit Overview</p></figcaption></figure>

## Increasing Messaging Limits <a href="#increasing_messaging_limits" id="increasing_messaging_limits"></a>

Business phone numbers are initially limited to 250 business-initiated conversations in a 24-hour moving period, but this limit can be increased.

{% hint style="warning" %}
Messaging limits are **not automatically increased**. Meta will analyze the messaging quality and activity to determine whether an increase is warranted.
{% endhint %}

* To upgrade out of Sandbox Tier, you need to send messages to **1,000+ unique contacts within a rolling 30-day** period or **verify your Meta Business Verification** anytime.
* Once a business is in Tier 1, the business’s phone number will be upgraded to the next tier if:
  * You are sending **high-quality messages** across all of your business phone numbers and templates.
  * In the last 7 days, your business has utilized at least **half of your current messaging limit**\
    \
    If your business phone number meets all conditions above, the messaging limit will increase by one level, 6 hours later.
* For top tiers (e.g., from 100K → Unlimited):
  * You’ll need to  send **100K or more messages** to unique contacts within a moving 24-hour period
  * The business phone number must have a **Medium** quality rating or higher.\
    \
    If you meet our eligibility requirements, we will automatically upgrade your business phone number to 1,000 messages per second within 12 hours.
