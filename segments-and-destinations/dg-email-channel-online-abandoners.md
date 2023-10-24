---
description: Dynamic Segmentation
---

# DG - Email Channel Online Abandoners

**Objective:** Dynamic segmentation solves the scalability problems marketers traditionally face when building segments for marketing campaigns or other use cases where setting up multiple variations of the same segment was required.

On an ongoing basis, the marketing team wants to remarket to customers who have clicked through an email offer to an online shopping experience, started the checkout process, but have not completed the Purchase.

The marketing team uses the Checkout and Purchase events for the website events and uses the Checkout event's sku variable to evaluate the sku name captured on the purchase. This assures it is the same item.

**Instructions:**

1. Navigate to Segment Builder in the left navigation and select **Create segment**
2. Click the gear icon to the right of Fields in the left pane\
   Verify ‘**Show full XDM schema**’ is selected

<figure><img src="../.gitbook/assets/Screenshot 2023-07-10 at 6.52.07 PM.png" alt=""><figcaption></figcaption></figure>

3. Click on the **gear icon** again to hide the setting
4. In the left pane, select ‘**Events**’ under **Fields**
5. In the **search box**, enter ‘**email clicked**’. Drag and drop into the segment canvas

<div align="left">

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-13 at 9.01.28 PM.png" alt=""><figcaption></figcaption></figure>

</div>

6. In the left pane, clear out the Search box
7. Under ‘**Event Types**’, locate ‘**Checkouts**’, and drag this to the segment canvas to the right of the ‘**Any**’ event

<div align="left">

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-13 at 9.02.15 PM.png" alt=""><figcaption></figcaption></figure>

</div>

8. In the left pane, locate ‘**Purchases**’ and drag this to the segment canvas to the right of the ‘**Checkouts**’ event.

<div align="left">

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-13 at 9.02.59 PM.png" alt=""><figcaption></figcaption></figure>

</div>

9. Your **segment** must look like this at this point:

<figure><img src="../.gitbook/assets/Screenshot 2023-07-10 at 7.07.25 PM.png" alt=""><figcaption></figcaption></figure>

10. Click on ‘**Checkouts**' in the segment canvas
11. In the left pane, search for '**SKU**'
12. Select the ‘**SKU**’ field and drag that into the ‘**XDM ExperienceEvent**’ container for ‘**Checkouts**’
13. Change the operator to “**exists**”

![](<../.gitbook/assets/Screen Shot 2022-12-13 at 9.04.36 PM.png>)![](<../.gitbook/assets/Screen Shot 2022-12-13 at 9.05.04 PM.png>)



14. Clear the search box. And Select '**Purchases**' event.
15. Search for ‘**SKU**’ and drag that into the ‘**XDM ExperienceEvent**’ container for ‘**Purchases**’
16. Clear the search box
17. Now, we are going to make this a dynamic segment. We will be using the **SKU** from previous events to make sure that that same **SKU** is being checked for the subsequent events in the **segment**. To make is easy for the users segment builder visualizes these parameters under 'Browse Variables' in the left panel

<figure><img src="../.gitbook/assets/Screenshot 2023-07-10 at 7.10.04 PM.png" alt=""><figcaption></figcaption></figure>

18. Select the **Checkouts1 | Product List Items 2** variable and drag and drop the SKU to the condition section that says 'Add to compare operants.
19. Change the ‘**XDM ExperienceEvent**’ container for ‘**Purchases 1**’ to ‘**Exclude**’
20. The dynamic condition should now look like this
21. At the top of the ‘**Events**’ canvas, update the time value to ‘**In last 1 day**’

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-13 at 9.06.09 PM.png" alt=""><figcaption></figcaption></figure>

22. Change the ‘**XDM ExperienceEvent**’ container for ‘**Purchases1**’ to ‘**Exclude**’
23. At the top of the ‘**Events**’ canvas, update the time value to ‘**In last 1 Day**’
24. Enter the segment name “**DG - Email Channel Online Abandoners - Initials**”.
25. **Save** the segment
