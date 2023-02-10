
## Prerequisites 

1. Previous knowledge of Figma
2. Be familiar with Power Apps
3. Have background assets, see step 14



## Step 1. Create the design in Figma

1. Goto to the [Microsoft profile in Figma](https://www.figma.com/@microsoft)
![[Pasted image 20230209141706.png]]
2. Scroll down and choose "Microsoft Power Apps", which is the **Figma UI Kit**
![[Pasted image 20230209141739.png]]
3. Click on the top right button "Get a copy", so get a copy of the UI toolkit in your Figma profile
![[Pasted image 20230209142559.png]]
4. This deploys a copy of the UI Tookit in your Figma workspace
![[Pasted image 20230209143950.png]]

5. Click on the plus button to create a new page for the Figma app
![[Pasted image 20230209144353.png]]
6. Rename the name space to a name of your liking. We used "Workspace"
![[Pasted image 20230209144544.png]]
7. Go to the Assets tab, as indicated in the figure and switch there 
![[Pasted image 20230209144758.png]]
8. Choose the Phone assets to build the app
![[Pasted image 20230209144920.png]]
9. Choose and drag to the Canvas, the Phone/Screen asset and resize it
![[Pasted image 20230209145108.png]]
![[Pasted image 20230209145557.png]]
10. Create 3 copies of this screen, by copying and pasting them pressing Ctrl + C or Cmd + C:
![[Pasted image 20230209145648.png]]
11. Next, dettach the instances, by right clicking on every one of the Screens and choosing Detach instance
![[Pasted image 20230209145907.png]]

12. Change the title of the screens, by selecting them. We rename them as 
	1. Welcome Page
	2. Subscribe Page
	3. Thank you Plage
![[Pasted image 20230209150055.png]]
13. In the Figma toolbar, click on the small rectangle icon, and choose "Place image"
![[Pasted image 20230209150227.png]]
14. Add the image to your canvas and center it over the leftmost screen:
![[Pasted image 20230209150747.png]]
15. Copy and paste the image over the other two remaining screens
![[Pasted image 20230209150848.png]]
16. From the panel on the left, grab the label asset and drag it to the leftmost screen
![[Pasted image 20230209151056.png]]
17. Add the text "RESERVATION APP" to the label, and proceed to place it where desired
![[Pasted image 20230209151350.png]]
18. You may also change the color as you desire
![[Pasted image 20230209151432.png]]
19. From the asset panel to the left, choose the Button asset and added to the leftmost screen
![[Pasted image 20230209151556.png]]
20. Modify the design to the button to fit your design. We used a white background and lila text
![[Pasted image 20230209151709.png]]
21. Copy and paste the labels on the leftmost screen, and add them to the center screen. Change the text as it suits you:
![[Pasted image 20230209151836.png]]
22. From the asset panel to the left, search now for the Phone/03 Textinput, Dropdown, ... and drag and drop to the screen the text input field
![[Pasted image 20230209152353.png]]
23. Copy and paste the text field two more times, to get the Last Name and Email address
![[Pasted image 20230209152503.png]]
24. Drag from the asset panel to the left, the Dropbox component
![[Pasted image 20230209152619.png]]
25. We rename the text inside all these components to "Name", "Last Name", "Email:someone@domain.com" and "Select a place category"
26. Copy the button from the leftmost screen and paste it in the center screen:
![[Pasted image 20230209152907.png]]
27. Paste the label to the rightmost screen and rename it:
![[Pasted image 20230209153013.png]]
28. Get an image from your computer, express your love :)
![[Pasted image 20230209153153.png]]

## Step 2. Import the design in Power automate

1. Head to the [Power Automate Portal](https://make.powerautomate.com)
![[Pasted image 20230209153722.png]]
2. Choose Figma Preview
![[Pasted image 20230209153803.png]]
3. Write a title for your Power App in the Popup that opens, then move to Figma to grab the Link to Figma page
![[Pasted image 20230209153909.png]]
4. Return to Figma, right click on the Page you created for your App, in our case, Workspace, and from select "Copy link to page"
![[Pasted image 20230209154215.png]]
5. Paste the link in the Link to Figma page or frame, in the Dialog you have open in Power Automate:
![[Pasted image 20230209154324.png]]
6. Switch to Figma to grab now the Figma personal access token and click  on the top right, where your profile is. Then choose settings. You will get this Dialog:![[Pasted image 20230209154635.png]]
7. Copy the token. Notice, that this is the only chance to grab to the token, after this, you will have to regenerate the token.
8. Paste it back in Power Apps, under the Figma personal access token section:
![[Pasted image 20230209154754.png]]
9. Choose the format as Phone to keep it consistent with the choice you did in Figma
![[Pasted image 20230209154844.png]]
10. Click create
11. Power Apps  will begin to import assets and create your app:
![[Pasted image 20230209154945.png]]


## Building the App in Power Apps

1. Finally the app, with its design it is imported in Power Apps 
![[Pasted image 20230209210957.png]]
2. Choose the Make button and in the formula field, enter ``` Navigate(Subscribe_Page)``` function, on the OnSelect event, as shown below:
![[Pasted image 20230209211416.png]]
3. Go to the Subscribe page, on the left panel, select it, and then clicking on the Send button, add on the OnSelect event, the function ```Navigate(Thank_you_Page)```
![[Pasted image 20230209211805.png]]
4. Fix the labels size if necessary:
![[Pasted image 20230209212058.png]]
5. Go now and try the app
![[Pasted image 20230209212207.png]]

And now you have the scalfolding to being to add functionality to your app. 

Happy coding!

