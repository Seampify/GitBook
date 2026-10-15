# How to trigger Automation from CTWA ads

This is a guide to show you an example on how to trigger an automation from [Clicks-To-WhatsApp-Ads (CTWA)](how-to-setup-ctwa-ads-from-ads-manager.md).

After creating an automation, you need to set up the trigger. There are 2 ways on how you can trigger the automation for your CTWA ads.

1. [Pre-filled message.](how-to-trigger-automation-from-ctwa-ads.md#how-to-trigger-automation-using-ctwa-a-ds-pre-filled-message)
2. [Ad ID.](how-to-trigger-automation-from-ctwa-ads.md#how-to-trigger-automation-using-ctwa-a-ds-id)

{% hint style="info" %}
If you have not setup an automation, [you may view here on how to import Automation template](../../seampifys-modules/automations/import-automation-template/)
{% endhint %}

### How to trigger automation using CTWA ads pre-filled message.

Double click on the trigger nodes and setup as follows:\
Trigger Condition: **Message text include any of keywords** \
Text keywords: \<pre-filled message you have set>

<figure><img src="../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Click here to learn how to [setup pre-filled message for CTWA](how-to-setup-ctwa-ads-from-ads-manager.md#setup-pre-filled-message-for-ctwa)
{% endhint %}

### How to trigger automation using CTWA ads ID.

Another way to trigger an automation is by using Ads ID. You can get this ID from your ads manager links.\
\
For example: [https://adsmanager.facebook.com/adsmanager/manage/ads/edit/standalone?act=XX\&business\_id=XX\&global\_scope\_id=XX\&date=XX\&insights\_date=XX\&selected\_campaign\_ids=XX&**selected\_ad\_ids=XX**\&sort=spend\~0\&current\_step=0](https://adsmanager.facebook.com/adsmanager/manage/ads/edit/standalone?act=247145454636129\&business_id=101178246298689\&global_scope_id=101178246298689\&date=2025-08-23_2025-09-22%2Clast_30d\&insights_date=2025-08-23_2025-09-22%2Clast_30d\&selected_campaign_ids=120231752139340766\&selected_ad_ids=120231755884990766\&sort=spend~0\&current_step=0) where u can get the ID from **selected\_ad\_ids**.

After that, you need to set your trigger as follow:\
Trigger Condition: **Custom Condition**\
Payload Key: **Referral Source Id**

Operator: **Is Any One**

Match String: **\<your\_ads\_id>**

<figure><img src="../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>
