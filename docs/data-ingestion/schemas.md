---
description: >-
  Schemas define the structure of the data to be ingested. This lab will walk
  through the steps to create an Individual Profile based schema.
---

# Schemas

Our goal here is to understand the schema composition. Different Schemas types, identity namespaces. Understanding this concept will become important when ingesting data into the platform. &#x20;

## Browse an Individual Profile Based Schema

1. Navigate to **Schemas** under Data Management in Adobe Experience Platform UI, then click browse.&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/image.png" alt=""><figcaption></figcaption></figure>

2\.  Search for the schema "DG - Customer Profile Schema":&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-10at5.07.27PM.png" alt=""><figcaption></figcaption></figure>

3\. Click on the schema Name to browse the schema configuration screen:&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-10at5.08.52PM.png" alt=""><figcaption></figcaption></figure>

## Schema Class

1. Click on the class: XDM Individual Profile. This shows what as a bare minimum a profile schema requires to create a profile in our system.&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-10at5.12.54PM.png" alt=""><figcaption></figcaption></figure>

1. After reviewing the profile class, let's start reviewing a field group Click on "Profile Core V2", and expand the schema tree. This action filter out anything outside of the Profile Core v2 field group. &#x20;
   1. Once you get the field group selected, feel free to click on an individual attribute to see its configurations pane.&#x20;
   2. This is very important because it tells the platform what type of data will go inside of that individual attribute. This allows to maintain data to be fully actionable by the marketer by formalizing data handling.&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-10at5.23.44PM.png" alt=""><figcaption><p>Field groups can be created by the customer or the customer can leverage out of the box field groups. If you decide to use an out of the box field group, you can remove fields you will not use on your schema and only bring what is relevant to you. Ultimately, you can define a custom field group of your choice. You can use field groups you create in other customer profile schemas. </p></figcaption></figure>

## Reviewing Identities

1. Make sure you unchecked the field group you had selected.&#x20;
2. Click on the identities listed on the schema composition pane.&#x20;
3. Notice it will expand the attribute that was label as an identity.&#x20;
4. There are 2 types of identities types: **Primary** and **non-primary**. Primary means that any data supplied will guarantee to always have for every record the primary identity. _For instance, in our demo the primary ID is customerDGID._ But we might or might not receive a "gigyaId" or a "BridgId". &#x20;
5. After selecting the namespace, you'll see the Field Properties pane, if you scroll down the pane, you'll see the identity configuration check boxes and dropdown.&#x20;
6. Remember, you might use out-of-the-box identity namespaces or create your own based on the type of id you are supplying (User level ID vs Session Level ID vs etc).&#x20;

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-10at5.32.39PM.png" alt=""><figcaption></figcaption></figure>

**Congratulations!** You have completed this module. Make sure to visit the lab takeaways section to expand on your knowledge on best practices for data modeling and other feature not covered in this lab.

