# Creating a Journey

## Let's create a basic Journey

The journey we will create will look like this:

<figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.02.17PM.png" alt=""><figcaption></figcaption></figure>

### Steps:

1.  Click on the grid icon on the top right corner of the user interface, and select the Journey Optimizer mode.&#x20;

    <figure><img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at2.59.00PM.png" alt=""><figcaption></figcaption></figure>


2. You will be redirected to the journeys mode homepage. From here, let's click on Journeys.&#x20;
3. Once you see the list of all the journeys we created for the demo, let's click on Create Journey button. Top right corner.&#x20;
4. Give a name to your journey: "Geo Location - Store Entry - Your initials." and click OK. \
   <img src="https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.05.45PM.png" alt="" data-size="original">
5. From the left menu inside the Journey Canvas, under events, select the real-time event called: GD\_Store\_Entry and drag it into the canvas, and then click ok.\
   ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.07.08PM.png>)
6. Next, let's add a condition from the same left hand side pallete, under Orchestration menu, expand the menu, and click on Condition to drag it into the canvas connecting it to the DG\_Store\_entry.\
   ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.09.33PM.png>)
7. Add a label "Cart Abandon?", then click on the Expression text field.\
   ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.11.04PM.png>)&#x20;
8. Within the expression editor, expand the Segments option, and drag the DG - Cart Abandoners or the DG - Cart Abandonment in the last day segment you created earlier. Either will work out for our exercise.\
   ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.13.13PM.png>)&#x20;
9. Click Ok. Then Ok to get back to the Condition Menu at the canvas.&#x20;
10. Then Check the box: Show path for other cases than the one(s) above. Notice how a new path is enabled. \
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.14.47PM.png>)
11. Change the name on both paths. For Path1, give the name YES, and on Others, label NO. Then click Ok to get back to the canvas.\
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot 2023-07-12 at 3.16.04 PM.png>)
12. Once back in the canvas. Let's add custom Actions. Drag onto the Yes path, the Action called Responsys\_Push.
13. Then, grab the custom Action called, Responsys\_Email&#x20;
14. Let's give it a label: Back in Stock?, and click on the Expression Editor.&#x20;
15. This time, let's expand the Source called DG\_Inventory\_System.&#x20;
16. Notice that we got warning on both nodes. If you click on the exclamation point at the top right to the Test Toggle. Most of the errors are because we haven't finished the configurations of the nodes. \
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.24.29PM.png>)
17. Click on the Responsys\_Push node. On the Action config pane, let's scroll down to find Request Parameters. These are all the fields Responsys is expecting us to pass, but we need to give data to each.
18. Click on the campaign field and on the expression editor, let's click on Advance Mode. Open Quotes and add the following: "Reminder Cart Abandon", then click OK. \
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.28.35PM.png>)
19. Next, on the expression editor, in the search field, Type: First Name. Then click the check box next to the First Name field, and click OK. \
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.30.46PM.png>)
20. Let's do the same thing but for the Last Name. On the expression editor for LastName, let's search for it in the search field, check the box next to the Last Name field, and click ok.
21. Let's repeat on Channel. Search for the Channel field on the search bar. Check the box. Click ok.\
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.32.47PM.png>)
22. Let's repeat the process, but this time we will search for a user ID in the profile. Search for: DG Customer ID. Check the box, and click ok.
23. Let's repeat the process for the field Content. Let's search for Favourite Category. Let's check the box and click okay.\
    ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.39.58PM.png>)
24. Finally, let' scroll up on the Action configuration pane, and click ok.
25. Repeat steps 18 thru 24 after clicking on the Responsys\_Email node. ![](<https://adbecdn.azureedge.net/labs/archbee/DGAdobeExperiencePlatformMulti/Screenshot2023-07-12at3.42.40PM.png>)
26. Congratulations, we just created your first journey.
