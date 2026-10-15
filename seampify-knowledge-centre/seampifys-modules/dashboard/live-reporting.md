---
description: >-
  This dashboard page provides an overview of live agent activities and
  performance metrics. Here's a detailed explanation of the key components:
---

# Live Reporting

<figure><img src="../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>

This page is focused on monitoring and managing live chat operations. It provides real-time data about:

* Agent availability and workload.
* Key performance indicators for response and resolution times.
* Department-specific queues and detailed agent activity.



## **Agent Status**

This section summarizes the status of agents handling live interactions:

* **Total Agents**: The total number of agents available in the system (e.g., 1 agent).
* **Online Agents**: The number of agents currently online and available to handle chats (e.g., 1 agent).
* **Offline Agents**: The number of agents who are have [set as offline](./#changing-your-online-status) currently and unavailable to handle chats (e.g., 0 agents).

<figure><img src="../../.gitbook/assets/image (706).png" alt="" width="265"><figcaption></figcaption></figure>

***



## **Performance Metrics**

These metrics provide insights into the efficiency of agent responses:

* **Avg. First Response Time**: The average time agents take to send the first reply to a customer's query. Currently, it is `0.00 seconds`, indicating no chats have been processed yet.
* **Avg. Response Time**: The average time agents take to respond to customer messages during the conversation. This metric also shows `0.00 seconds`, likely due to no active chats.
* **Avg. Closing Time**: The average time it takes to resolve and close customer chats. Again, this is `0.00 seconds` in the absence of interactions.

<figure><img src="../../.gitbook/assets/image (707).png" alt="" width="563"><figcaption></figcaption></figure>

***



## **Live Agent Queue**

This section displays the number of chats waiting in the queue for each department:

{% hint style="warning" %}
You will need to [create department](../settings/business-settings/department.md#create-a-department) first to have data for this section.
{% endhint %}

* **Department Name**: Lists all the departments configured in your Seampify account.
* **Total Chats**: Indicates the number of chats currently queued for that department (e.g., 0 chats).
* **Action**: Provides a summary of contacts under that department.

<figure><img src="../../.gitbook/assets/image (709).png" alt=""><figcaption></figcaption></figure>

***



## **Live Agent Report**

This section details the live agents and their activities:

* **Name**: Displays the name of the agent.
* **Email**: The email address associated with the agent account.
* **Concurrency**: The maximum number of chats the agent can handle simultaneously. This can be set under [Teams](../settings/business-settings/teams.md#adding-a-team-member).
* **Assigned**: The number of chats currently assigned to the agent.
* **User Status**: Indicates whether the agent is online or offline.
* **Action**: Similar to the queue section, this provides Agent summary (Agent Name, contact number and the duration each agent spent on chats.)

<figure><img src="../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

***

