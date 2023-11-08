---
description: This lab will walk though the data ingestion workflow in the UI.
---

# Data Ingestion

## Download sample csv data for the exercise

Download and review the sample Loyalty file from the[ Lab Data ](lab-data-ingestion.md)section. This data is a sample representation of the  some fields you would source from your in-house systems to feed  business cases. We are keeping things small to fully understand the ingestion process.

## Ingesting .csv data in adobe Experience Platform

1. Navigate to the **Workflows** section through the left panel
2. Click on the **Map CSV to XDM schema** card
3. Click **Launch** in the right panel

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/ScreenShot2022-12-12at2.16.17PM1.png" alt=""><figcaption></figcaption></figure>

&#x20;4\.  Select the **Existing Dataset** option

&#x20;5\.  Search and select your **dataset** by name from the dropdown (You created this dataset before)

&#x20;6\.  Enable **Partial Ingestion**. Set threshold to the default 5%

&#x20;7\.  Update the **Dataflow** to include your initials

&#x20;8\.  Enable all alerts

&#x20;9\. Click **Next**

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-10 at 6.17.31 PM.png" alt=""><figcaption></figcaption></figure>

&#x20;10\.  **Upload the .CSV file provided**. Drag & Drop or click **Choose files to upload**.

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-10 at 6.06.15 PM.png" alt=""><figcaption></figcaption></figure>

### Mapping source columns to XDM schema fields

1. As you proceed into the field mapping step, a couple of things to note;

* This mapping step is a requirement to ingest delimited files ONLY. **Parquet** and **JSON** formatted files can be dragged and dropped into the appropriate dataset since they are key value pairs and do not need to be explicitly mapped.
* Adobe Experience Platform's AI has correctly mapped most the source fields to the best matched **XDM schema field**.&#x20;

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-10 at 6.07.26 PM.png" alt=""><figcaption></figcaption></figure>

Navigate to **Datasets**

<div align="left">

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screen Shot 2022-12-13 at 10.25.01 AM.png" alt=""><figcaption></figcaption></figure>

</div>

Search and select your newly created **dataset**

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-10 at 6.10.37 PM.png" alt=""><figcaption></figcaption></figure>

Notice a **batch** is created as a result of the ingestion **workflow** that was triggered

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screen Shot 2022-12-13 at 10.25.23 AM.png" alt=""><figcaption></figcaption></figure>

Once the status for the batch says **"Success"**, you can Preview the **Dataset** by clicking on the **Preview Dataset** button on the top right of your screen.

This allows for validation of source columns to **XDM schemas.**&#x20;

<figure><img src="../https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-10 at 6.11.40 PM.png" alt=""><figcaption></figcaption></figure>



