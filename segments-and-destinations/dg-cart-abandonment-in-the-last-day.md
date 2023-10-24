---
description: Sequential segmentation
---

# DG - Cart Abandonment in the last day

In this exercise, we'll use experience events to build a sequential segment.

1. In the left-hand navigation panel, click Segments.
2. In the top right corner of the screen, click **Create Audience**. Click **Build Rule.**

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-12 at 7.33.16 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-12 at 7.16.48 PM.png" alt=""><figcaption></figcaption></figure>

3. Under **Fields,** click **Events.**
4. Within Events, search for the following eventType: Product Views.
5. Drag and drop the **Product Views** eventType field into the segment canvas.

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.24.30 AM.png" alt=""><figcaption></figcaption></figure>

6. In the same way, under events search for the eventType **Product List Adds**, but this time drag it just right after the **Product Views.** A blue line will appear on **Product Views.** When you see it, drop the Product List Adds like the following screenshot:

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.28.10 AM.png" alt=""><figcaption></figcaption></figure>

7. In the same way as the other 2 events, now search for **Checkouts** on the search bar, and drag and drop the **Checkouts** right after **Product List Adds** like this:

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.30.05 AM.png" alt=""><figcaption></figcaption></figure>

8. Finally, search for the following event using the search bar: **Purchases** right after **Checkouts** like this:

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.31.23 AM.png" alt=""><figcaption></figcaption></figure>

* Apply recency to your segment rule by clicking **Anytime**.&#x20;
  * In the dropdown, select **In the Last **<mark style="color:purple;">**1**</mark>** Day**

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.32.12 AM.png" alt=""><figcaption></figcaption></figure>

9. Lastly, click on the Purchase event listed on your Sequence of events, and make sure the event rule is Excluding. This will exclude any user that matches the sequence and has completed the purchase. We want to target people who did the following sequence of events but has never completed the purchase. Your segment should look like this now:

<figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 9.34.44 AM.png" alt=""><figcaption></figcaption></figure>

10. Name your segment: DG - Cart Abandonment in the last day - **Initials**
