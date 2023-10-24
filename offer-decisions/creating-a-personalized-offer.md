---
description: This lab will walk through the steps needed to create a personalized offer.
---

# Creating a Personalized Offer

## Create a Personalized Offer

1. From the left navigation menu, under Decision Management, click on the **Offers** option.
2. Click Create an Offer button and chose **Personalized offer** option.  ![](<../.gitbook/assets/Screenshot 2023-07-12 at 11.34.01 AM.png>)
3. For the name of Offer, type: "25% Coupon - Initialss"
4. Add a start date and an end date of your choice.&#x20;
5. Under Collection Qualifiers, please start typing the collection qualifier you created in the previous lab "Placements and Collection qualifiers". Once it shows, click on the name.&#x20;
6. You may leave the offer attributes empty. However, these are additional metaData that you can decorate your offer with. For example, if this offer is going to be consumed by a third party or via the API. They can use those values for specific reporting needs, or logic needs on that system. Typically, users would use this for internal campaign codes, or tracking names. These key values pairs are free form and everything is stored as a string.&#x20;
7.  Your Personalized offer should look like this. If so, Click Next.&#x20;

    <figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 11.39.34 AM.png" alt=""><figcaption></figcaption></figure>


8. On Representation 1, you can select the channel **Email,** then select the placement we created on the previous lab.&#x20;
9. From the asset library, click browse and select an image from the asset essentials folder. \
   ![](<../.gitbook/assets/Screenshot 2023-07-12 at 12.48.52 PM.png>)
10. Provide a destination link for example: https://experience.adobe.com. This is where our offer will lead users after clicking on our offer.&#x20;
11. Once you are done, you could add another representation to make this offer available to more than one channel. This step is not necessary as we aren't learning anything new.&#x20;
12. Your offer Representations should look like this. If so, Click Next.\


    <figure><img src="../.gitbook/assets/Screenshot 2023-07-12 at 1.49.57 PM.png" alt=""><figcaption></figcaption></figure>


13. Once you are in constraints, click on the option: "Visitors who fall into one or multiple segments" and select one or all the segments we created during the Segmentation Labs.&#x20;
14. For our lab, toggle the option to exclude capping constraints.  and leave priority as 0. click next.\
    ![](<../.gitbook/assets/Screenshot 2023-07-12 at 1.54.46 PM.png>)\


{% hint style="info" %}
Capping is an important feature because you can control how many times should this offer needs to be shown to a user. It can be in total number of impression, or per profile. You can also cap by a custom event (Like purchases) to remove the user from seeing this offer if he does indeed makes a purchase. You can apply a frequency to clear and repeat the capping after an specific period of time. Lastly, capping constraints can be applicable across placements or only specific ones.&#x20;
{% endhint %}

15. Congratulations, you reach the review step. Check your offer looks similar to this one and then click Finish and approve.\
    &#x20;![](<../.gitbook/assets/Screenshot 2023-07-12 at 1.56.42 PM.png>)
