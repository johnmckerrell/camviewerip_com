---
layout: page
title: Features
---

## Audio Support

Audio support is available as an in-app purchase, which supports my time spent developing this and other functionality within the app. The app does now support 2-way audio although this isn't working perfectly on all cameras at the moment, the audio received from the cameras can be noisy and sending audio to the cameras can also be problematic. A large part of this is due to the camera but there's definitely some improvements that I can make in the app to improve this.

## Proxy Safer Mode

To support the audio functionality the app communicates with the camera using its own non-standard protocol. Sometimes this will not work, most often if you are connecting to the camera through a proxy server. You may not even be aware that your device is accessing the internet through a proxy server, many mobile and cell networks insert a transparent proxy into your web communications. Using Proxy Safer mode forces CamViewer to only use HTTP, the standard web protocol, to communicate with your camera. While this should allow you to connect through a proxy it will mean that you cannot use audio functionality. The app now attempts to detect proxy servers and switch to Proxy Safer mode but this will not always be possible so if you're having problems, you might like to switch to this mode yourself.

## Basic Image Mode

While I try to support as many cameras as possible, it's impossible to catch all of them. I've now added a "Basic Image" mode which will hopefully help in these circumstances. If you can get an MJPG feed or a JPG snapshot out of your app then put the link to that into CamViewer and it will display the image. It will keep requesting the image while you watch, simulating a live video feed. If your camera supports it you can put the username and password into the path, if your camera supports HTTP Auth then you can enter the username and password into CamViewer and it will use them. See more information on the [Getting Started](/getting-started) page.

## Digital Zoom

Digital zoom allows you to scale up the images received by the camera to get a closer look at an area. In portrait orientation you can simply use the standard pinch gesture and swipe to look around once zoomed in. When in landscape orientation you will need to disable the pan/tilt controls before you can use the pinch and swipe gestures. ![](/g/Features/controls-disabled.png){:class="right"} This is done using an icon that is only available in portrait mode on iPhones but will show up in the navigation bar on the iPad.

## Optical zoom

For cameras that support it, CamViewer now allows you to use the optical zoom to get a closer look. Look out for the magnifying glass icons which should show up, tap one to zoom in and the other to zoom out.

## Presets

![](/g/Features/presets.png){:class="right"} CamViewer will let you set and access 10 presets on webcams that support it. Simply tap the icon and follow the instructions.

## Data Usage

CamViewer will give you an indication of the amount of data that you're using when viewing your cameras. These cameras can use large amounts of data so it's good to keep an eye on them!

## Access to Parameters

CamViewer allows you to turn on the I/O function if your camera has it or alternatively will let you turn the Infra-red lights on and off, again if your camera's interface supports this. You can also set other parameters including brightness and contrast to improve the image you're getting from your camera. The list of parameters that you can access will develop more over time.

## [Duplicate](duplicate)

## [RTSP](rtsp)

