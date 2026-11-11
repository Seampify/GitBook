# Google Sheet

In Seampify, we have already integrated with Google Sheet. With this function, you will be able to seamlessly collect any attribute datas into a Google Sheet without any further settings needed.<br>

### How to Activate Google Sheet Integration

{% stepper %}
{% step %}
#### Go into settings on Seampify and navigate into Integration.

<figure><img src="../../../../.gitbook/assets/google sheet gitbook.PNG" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Now Select Google Sheet

<figure><img src="../../../../.gitbook/assets/google sheet gitbook2.PNG" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Now press Save.

<figure><img src="../../../../.gitbook/assets/image (796).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Ensure that this is enabled.

<figure><img src="../../../../.gitbook/assets/image (798).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}



### How to use Google Sheet in an automation

Here is a simple guide to use this integration in an automation.\
\
**Step 1:** \
When you open an automation. You can go into the action button and scroll down you can see a new node called " add new row in Google Sheet"

<figure><img src="../../../../.gitbook/assets/google sheet gitbook3 (1).PNG" alt=""><figcaption></figcaption></figure>

**Step 2:** \
Next, we can go into node and we will see this node setting.

<figure><img src="../../../../.gitbook/assets/google sheet gitbook4.PNG" alt=""><figcaption><p>Node settings</p></figcaption></figure>

**Step 3:** \
Now, we will need to fill up the details of the node settings.

<figure><img src="../../../../.gitbook/assets/image (799).png" alt=""><figcaption></figcaption></figure>

* **Google Service Account :** This is an auto-generated service account that is used to give access to Seampify to write data into your Google Sheet. You will need to grant an Editor role access to this Google Service Account.
* **Google Sheet Url:** Enter the link to your Google Sheet here. Seampify will send and add new data into this sheet.
* **Google Drive Url:** Enter the link to your Google Drive folder here. This is only needed if you have any fields that collect file uploads — the uploaded files will be stored in this Drive folder.

**Step 4:** \
Now, you need to map the Attribute data to your Google Sheet column name.\
\
Click the **"Source Attribute"** dropdown to select which attribute data you want to send to the Google Sheet.\
\
Then, type the corresponding column header name into the **"Google Sheet Column Name"** field.\
\
You can ignore the **Field Type** section.

<figure><img src="../../../../.gitbook/assets/image (800).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Make sure the **Google Sheet Column Name** exactly matches the header name in your Google Sheet, and do not leave out any columns. This ensures that the data can be transferred smoothly without any issues.
{% endhint %}

**Step 5:** \
Add timestamp. (Optional)

You can add a timestamp to your Google Sheet to log when each data entry is added.\
\
To do this, scroll to the bottom until you see the section of "**Auto Add Timestamp in Sheet**" and enter the header name of the column where you want the timestamp to appear.

![](<../../../../.gitbook/assets/image (802).png>)

{% hint style="danger" %}
Make sure the **Google Sheet Column Name** exactly matches the header name in your Google Sheet. This ensures that the data can be transferred smoothly without any issues.
{% endhint %}

<br>

**Step 6:** \
Update Node to save the settings created.\
![](<../../../../.gitbook/assets/image (803).png>)
