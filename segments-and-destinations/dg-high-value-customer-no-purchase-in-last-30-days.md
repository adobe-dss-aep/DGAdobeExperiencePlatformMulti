---
description: Hybrid Segmentation
---

# DG - High Value Customer - No purchase in last 30 days

In this exercise, we'll combine experience events and profile attributes to build a hybrid segment.

1. In the left-hand navigation panel, click Segments.
2. In the top right corner of the screen, click **Create Audience**. Click **Build Rule.**

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

3. Under **Fields,** click **Events.**
4. Within Events, under event Type search for the following data field path\
   **Purchases**\
   Alternatively, you can search "purchases" in the search bar.
5. Drag and drop the **Purchases** field. Click on the Rule, then change Include to Exclude. Then change the time for the purchase event evaluation. In this case, we will need to evaluate all events in the past 30 days. We will exclude users that have a purchase event, but will include the ones that do not have a purchase event.
6. In the **Fields** bar, select **Attributes.**
7. Search **for the word: Points**
8. Drag and drop the **Points** field into the canvas
9. Change the operator to **is greater than or equal to.** Enter **850.**

<figure><img src="../.gitbook/assets/Screenshot 2023-07-10 at 6.32.22 PM.png" alt=""><figcaption></figcaption></figure>

10. Name your segment: "DG - High Value Customer - No purchase in last 30 days - **INITIALS**"
