---
description: >-
  This guide outlines how to upload a contacts database in bulk using CSV and
  manage attributes for effective organization in the platform.
---

# Uploading Contact Database

{% embed url="https://youtu.be/4XGBv4RFuAg" %}

## **Uploading Contacts in Bulk**

To upload contacts in bulk, follow these steps:

### Step 1: Navigate Contacts&#x20;

* Go to "Contacts" tab&#x20;
* Click "Import CSV" button

<figure><img src="../.gitbook/assets/image (376).png" alt="" width="563"><figcaption></figcaption></figure>

### Step 2: Upload Contacts&#x20;

* If the file already has a country code for the contacts, you can tick **Yes** under the Phone Number have country code checkbox. Otherwise, select the country code that you wish to add for all the numbers in the CSV file.

{% hint style="danger" %}
Seampify can only add ONE country code to all of the numbers in a CSV file. If you have multiple country code, please upload the CSV file separately.
{% endhint %}

* Add a tags (if required) for all the contacts in the CSV file. Click "Add" to save the tag.

<figure><img src="../.gitbook/assets/ScreenRecording2025-01-21155908-ezgif.com-video-to-gif-converter.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Note: This tagging feature is useful for filtering broadcasts by specific tags in the future.
{% endhint %}

<figure><img src="../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>

* Upload CSV file and you'll see some of your contact numbers and other details in the Preview Import.

{% hint style="warning" %}
Kindly only upload CSV file format. You may click on the Download Sample File to view the CSV template.
{% endhint %}

<figure><img src="https://lh7-rt.googleusercontent.com/slidesz/AGV_vUfTC_LJY5OPwoPq-nBYSBGuCgWXeAZsJK1YcrlSeaSR7TBJfdr6TBuQEzG6klEiaTpMghAQJBoDD4qpIA-Lgg7YUnGw4Ka08hshaufZbV24Tm5cBIgLXhZ_n8fRqopMWHtpIUUXWwvJcKH0wWdWMh_xm64NzYs=s2048?key=YuKrnlkH4ooGPnQJnGpRUA" alt=""><figcaption></figcaption></figure>

* Tick the **"Data has headers"** option if your CSV file has a header and it will skip the first row.
* Click **Next**.

### Step 3: Data Validation

* Check that all data column are mapped to the correct Contact Fields.
* By default, the column will be assigned to the respective Contact Field if the name is matched . You can manually drag data into the correct Contact Field boxes if needed.

{% hint style="info" %}
Note: If you need to add a new Contact Field, please do this step beforehand. You may refer [how to add a Contact Field here.](../seampifys-modules/contacts/filter-options/contact-fields.md)
{% endhint %}

<figure><img src="../.gitbook/assets/image (271).png" alt=""><figcaption></figcaption></figure>

* Click **Next** once all data is aligned.

### Step 4: Complete Import

* It'll take a few moments to upload the contacts, and once the process is completed, you can click **Finish**.

<figure><img src="../.gitbook/assets/image (380).png" alt=""><figcaption></figcaption></figure>



## **Things to Note before Uploading CSV File:**

### **Mandatory Data in CSV**

* **Phone Number** - this is the unique identifier for each contact
* **Full Name** - Without a name, managing your chats becomes difficult since each conversation will appear nameless like this:

<figure><img src="../.gitbook/assets/Screenshot 2024-11-15 at 7.36.24 PM.png" alt="" width="115"><figcaption></figcaption></figure>

* It is recommended to add as much informations for each of your contact as possible. You may add columns in your Excel file such as Race, Birthdays, Language etc.&#x20;

{% hint style="info" %}
Note: Each column is named as Contact Field in Seampify. There are some default Contact Filed in Seampify, if you need to create a new Contact Field, please refer [how to add a Contact Field here.](../seampifys-modules/contacts/filter-options/contact-fields.md)
{% endhint %}



### **Avoiding Duplicate Values**

By default, Seampify will merge duplicated Phone Numbers but it is best to ensure no duplication in your data before uploading:

#### **Step 1: Check for Duplicates in Excel**

1. Open your **Excel sheet**.
2. Highlight the cells you want to check (e.g., **Phone Number**).
3. Navigate to **Home > Conditional Formatting > Highlight Cells Rules > Duplicate Values**.
4. Choose a formatting style to highlight duplicates and click **OK**.

#### **Step 2: Review and Adjust**

1. Carefully review all highlighted duplicates.
2. Make necessary adjustments to remove or differentiate duplicate entries.



### Adding Country Code to Your Numbers

You are able to send WhatsApp messages from worldwide hence it is a mandatary to include a country code for your numbers. If your data does not have a country code, Seampify is able to help you add a specific country code to all of your numbers during upload.&#x20;

* To do this, select No under Phone Number have country code? section and select the country code that you wish to add for all the numbers in the CSV file.

{% hint style="danger" %}
Seampify can only add ONE country code to all of the numbers in a CSV file. If you have multiple country code, please upload the CSV file separately.
{% endhint %}

<figure><img src="../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>
