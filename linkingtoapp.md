---
layout: page
title: Linking to the App
---

You can make it easier for people to launch CamViewer and have them automatically view a camera using the new URL support in [v1.9.16](/changelog#1916). An example URL would be:

    camviewer:///?address=http://webcam.example.com:8081/&name=Example+Cam&username=admin&password=supersecret&groups=Foo,Bar

That's `camviewer:///` followed by a query string with the following properties:

 * *name* - The name you want to display for the camera.
 * *address* - The address to access the camera on.
 * *username* - The username for accessing the camera.
 * *password* - The password for accessing the camera.
 * *groups* - A comma separated list of groups to add the camera to, otherwise the camera will be added to an "Auto Cams" group.

If no parameters are given, the app will simply be launched. If the username, password or address are **left off** then the "Edit Camera" screen will be displayed. If a username or password is not required then simply pass a blank value (e.g. `&username=&`). If no camera name is given then the name "Auto Cam" will be assigned. If a name already exists within the app, a number will be appended.

If a camera with the given address, username and password already exists, then this will be displayed and no new entry will be created.
