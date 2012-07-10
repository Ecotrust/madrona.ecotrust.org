---
layout: tutorial
title: Madrona Appliance Tutorial
active: developer
---

Madrona Appliance Tutorial 
=========================================================

<div class="alert alert-info">We assume you have already:
	<ul>
		<li><a href="{{BASE_PATH}}/developer/appliance/">Downloaded and installed</a> the Madrona Appliance</li>
		<li>Have the virtual machine (VM) up and running.</li>
	</ul>
</div>

This tutorial will walk through creating an app using the Madrona App Generator and then getting started customizing that app.  The apps created by the App Generator use the Google Earth Plugin, which is just one of the mapping clients that you can use with Madrona.  See the Madrona <a href="{{BASE_PATH}}/experience">experience</a> page for more examples and their full source code.

1. In your running VM, click the __Start Using the Madrona VM__ button
![Madrona VM startup screen]({{BASE_PATH}}/assets/img/tutorial/appliance/initvm.png)

2. The App Generator is now running.  Follow the instructions onscreen to configure your host system to send web requests for __madrona__ to the VM's IP address.
<div class="alert alert-info">This IP address could be different every time you start the VM, in which case you will need to change it.</div>
![Madrona VM instructions]({{BASE_PATH}}/assets/img/tutorial/appliance/hostsvm.png)

Creating the initial demo app 
---------------------------------------

Now that your networking is setup, access the Madrona App Generator from a web browser in your *host* operating system *not the VM*.

<div class="alert alert-info">Why access the App Generator from your operating system?  Because this version of the App Generator uses the Google Earth Plugin, which is not available for Linux.  So you will need to access it from a Windows or OSX host system.  This will change in the future when the App Generator uses a 2D mapping client.</div>

1. Open the URL *http://madrona/*

2. Sign in. The username and password are both *madrona*

3. Click the __Generate New Madrona App__ button to begin.

4. Provide the App with a name, we'll be using '*Test App*'' throughout this tutorial.

5. Enter the description '*Test Application*' or whatever you want.

6. __Draw__ a study region on the map.  The studyregion is used to define the geographical extent of your project.  For best results, draw a smaller region.

7. Under __Features__, select the __AOI__ feature.  
<div class="alert alert-info">Features are spatial entities that the user will be able to draw, edit and share with other people.</div>
8. (Optionally) Create one or more additional features by clicking the __+__ button.  Give them a name and a type (point, line, polygon or folder). Once you create more you need to __select__ them all in the __Features__ list by holding down the Ctrl key and selecting them all. 

9.  Select one or more of the available KML data layers to make available to your user.  

10. (Optionally) Click the __+__ button to add your own KML file if you know the URL.

11. Click the __Save__ button.  You should now see a summary of your app.
![App summary]({{BASE_PATH}}/assets/img/tutorial/appliance/appgen_new_or.png)

Initialize and Activate Your App
---------------------------------------

1. Click the __Initialize__ button.
<div class="alert alert-info">The initialization process can take up to a minute so be patient.  Under the hood this is generating the code for your app using some simple commands.</div>

2. Once initialization is complete, click the __Activate__ button.
<div class="alert alert-info">Under the hood this is configuring the Apache web server to make your app available on port 81.  You can only have one app active at a time.</div>
![Activate the app]({{BASE_PATH}}/assets/img/tutorial/appliance/appgen_or.png)

Test Out Your New App
---------------------------------------

1. In the admin, click the __Go To App__ button.  This will open a new tab and load your new app being served at *http://madrona:81/*.  When the app loads it will automatically zoom the map to the study region that you drew.  
<div class="alert alert-info">Loading may take a little while the first time as it caches your requests in order to speed up subsequent loads.  If you don't already have the Google Earth Web Plugin installed you will be asked to at this time.  Once you do, refresh the page</div>

2. Click the __Login__ button in the top right.  The username and password are both *madrona*

3. Click the __Data Layers__ icon in the top left.  
<div class="alert alert-info">This is next to the __Tools__ icon which looks like a gear</div>

4. You should see a *Test App* folder which has a data layer for your study region.  Try turning this on and off.  Double-click to zoom into it.

5. You should also see a *Base KML Data* folder which has all of the data layers that you added.  Try turning them on and off.

6. Now let's create some features.  Click the __My Shapes__ tab in the top left.  If you don't see this tab you probably aren't logged in and should go back to step 2.

7. Click the __Create__ button and then click __AOI__ which generically stands for *Area of Interest*.  

8. Click the __Draw Shape__ button and then draw a polygon on the map by clicking once for each vertice and the double-clicking the last point to finish.
<div class="alert alert-info">Madrona will now validate your shape, make sure you didn't draw any bowties or any other type of self-intersecting polygon.  If it's valid you now have the option of editing your shape or if you are happy click the __Next__ button.</div>

9. Give your new feature a name, any name.  Optionally, give it a description.

10. Click the __Submit__ button

11. You'll now be presented with detailed information for your feature.  Close this window by clicking the 'X'.

12. You should now see your feature listed under *Features and Collections*

13. Now let's create a new folder.  Do it the same way you created an AOI, through the __Create__ menu.

14. Once you create your folder and see it under *Features and Collections*, click and drag your feature into the folder.  This allows you to organize your features any way you like.
<div class="alert alert-info">There are many more things you can do with these features and folders out of the box including edit, delete, copy, share and download.  Try selecting one or more features or folders and performing these actions, for example download an entire folder of features as KML.</div>

Viewing and editing the generated code
---------------------------------------

To view the code behind this application that was generated by the App Generator using the information you provided, start by going back to the Virtual Machine window.

1. Click the __Start__ button in the lower-left, it's the button that looks a little strange.  Click __Start -> Accessories -> LXTerminal__ to open a command line terminal window

2. Now Click __Start -> Accessories -> Sublime Editor 2__ to open your text editor

3. In Sublime Text click __File -> Open Folder__

4.  Now open __/usr/local/userapps/testDemoProject/testdemoproject__
<div class="alert alert-info">In this step you are selecting and opening a folder which might seem a little strange.  By doing this Sublime gives you a view of the entire folder in the left panel letting you quickly open any file under it.</div>
![Terminal window]({{BASE_PATH}}/assets/img/tutorial/appliance/terminal.png)

<div class="alert alert-info">Nice work, next up:
    <ul>
        <li><a href="{{BASE_PATH}}/developer/tutorial/madrona_appliance_customize.html">Customize</a> your app</li>
    </ul>
</div>
