---
layout: page
title: FAQ - Frequently Asked Questions
---



1. "Why does my camera connect fine at home but not over 3G?"
    * This may be because you have not set up your camera to be available outside your home network. See the [Networking](/networking) page for more information on how to do this. If you can access your camera over other networks but not over 3G it might be because your mobile/cell network operator "proxies" the pages that you visit. In this case when you try to visit a website you actually connect to a server owned by your operator which then connects to the web server. This is ok for most web pages but can cause problems with IP cameras.

      Version [1.9.13](/changelog#1913) attempts to fix this problem by detecting the proxy and falling back to [Proxy Safer Mode](/features#proxy-safer-mode). The app will not always be able to detect this automatically so you might like to force Proxy Safe mode yourself by editing the properties for the camera and changing the Connection property. Unfortunately in this mode you will not be able to use the audio features but your camera's video feed and the controls should still work. This is most likely to occur if you are connecting to your camera on port `80`, using an alternative port may bypass the proxy and enable you to use the audio features. If the auto-detect feature causes problems, version [1.9.14](/changelog#1914) added a setting to allow you to disable this.

1. "Why does my camera show an error or disconnect after a few minutes of use?"
    * This is something I have not yet identified a cause for but it may be caused by accessing the camera through a proxy server which closes the connection after streaming video for a few minutes. Version [1.9.14](/changelog#1914) improves the situation by trying to reconnect to the camera automatically if the connection is lost. I will continue investigating this to attempt to find why disconnects might be happening though.

1. "Does the app use data in the background?"
    * When you put the app in the background, or lock your phone, the app will disconnect from the camera, so no it will not use data in the background.

1. I have multiple cameras and sometimes the app shows the right feed but sometimes it shows a feed from a different camera.
    * If you have multiple cameras you should operate them on different port numbers, so the first might be on port `8001`, the second `8002`, etc.

1. The app worked fine originally but has now stopped working after a period of time.
    1. Some DDNS services require you to reactivate your account after 30 days, check that the DDNS is still working.
    1. If you have just updated CamViewer you may find that you need to reboot your phone for it to keep working. This seems to be an issue that came in with version [1.9.14](/changelog#1914).
    1. Some of the cameras are quite cheap and can have issues meaning the camera itself might need to be rebooted from time to time.
    1. If you are not using DDNS then your IP address may have changed.
    1. If you have manually forwarded the camera's port on your router but not fixed the internal IP address, this may have changed.
