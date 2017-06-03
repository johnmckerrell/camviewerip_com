---
layout: page
title:  Unsupported Cameras
---

Unfortunately I haven't had time to get the app working with every IP camera that's available. Cameras with H.264, Dlink cameras and others seem quite popular but unfortunately won't be detected by CamViewer, **but** it can be possible to get a video feed from some of these cameras in CamViewer.

I've now added a "Advanced Direct Image" mode which will hopefully help in these circumstances. If you can get an MJPG feed or a JPG snapshot out of your app then you can put the link to that into CamViewer and it will display the image. It will keep requesting the image while you watch, simulating a live video feed. If your camera supports it you can put the username and password into the path, if your camera supports HTTP Auth then you can enter the username and password into CamViewer and it will use them. You will not be able to control the camera or access its properties or other features, but this way you will at least get a video feed.

With some H.264 cameras you can access the JPG snapshot at `http://yourcameraip:port/tmpfs/auto.jpg` - you will also need to enter the username and password for your camera.

I'm definitely intending to add support for more cameras, just struggling to find the time at the moment.
