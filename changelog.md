---
layout: page
title: Change Log
---

This page outlines the changes that were introduced in each version. I won't fill in too much history but will look to update this as the app develops. Most updates include various bug fixes but I'll only list the most important ones below.

## 2.1.2
### Released 28th February 2017
 * Fixes crash bug with Foscam-style cameras.

## 2.1.1
### Released 13th December 2016
 * Fixes crash bug when using 2-way audio.

## 2.1
### Released 23rd November 2016
 * Fixes a problem with encoding complex passwords and improves playback of HD/RTSP video.

## 2.0.1
### Released 28th June 2016
 * Fixes in-app purchase, and some general upgrades and bug fixes

## 2.0
### Released 2nd December 2015
#### iCloud Syncing Support!

 * Think of v2.0 as the El Capitan to 1.9.xxx's Yosemite. Lots of changes and improvements to the underlying code but not so many visual or functional changes. There have been some good functionality updates recently so I thought with those and the iCloud support in this version it was finally time to bump up to v2.0. I'm expecting the transition from v2.0 to v3.0 to take a lot less time than from v1.0 to v2.0!

 * I know I promised an icon update when v2.0 came along but it seems like Apple has finally caught up with the minimalism of CamViewer's UI (or at least they did back with iOS7) so the icon's hanging around, at least for a little while longer!

## 1.9.31
### Released 12th September 2015
 * Few bug fixes for "Turn switch on for 5s" feature, crash bug with problem reporting, and custom SSL certificates.

## 1.9.30
### Released 22nd August 2015
 * Some small bug fixes to Touch ID & passcode support.
 * This will be the last version to support iOS6.

## 1.9.29
### Released 4th August 2015
 * Another small bug fix update.
 * Support for [Tenvis iProbot 3](/supported-cameras) added too!

## 1.9.28
### Released 29th July 2015
 * Another small update mainly to fix problems with detecting that you have no Wi-Fi connection.
 * Also adds support for rtsp:// style URLs, [more info here](/features/rtsp)

## 1.9.27
### Released 11th July 2015
 * Just a small update to fix a problem with the media port being restricted to smaller numbers.

## 1.9.26
### Released 2nd June 2015
 * Touch ID Support! Set a passcode using the in-app Settings option and use Touch ID to secure your cameras. Secure the whole app, individual cameras, or just for editing cameras.
 * Support for a few cameras that have different streams and alternative media ports, and multiple cameras on one system. If you have a camera like this please get in touch.
 * Various bug fixes and small enhancements, upgraded RTSP support fixing crash bugs.

## 1.9.25
### Released 19th December 2014
 * Restoring iOS4 support which caused crashes in last version, this will be the last build to support iOS4.

## 1.9.24
### Released 25th November 2014
 * A few more small updates. Updating problem reporting. Fixing status bar on iPhone6, moved the flip and mirror buttons into the parameters section and added a refresh button for infrequently updating webcams.
 * Fixed a bug with the "camera slow to load" message and increased the timeout.

## 1.9.23
### Released 19th November 2014
 * A few more small updates. Fixing status bar on iPhone6, moved the flip and mirror buttons into the parameters section and added a refresh button for infrequently updating webcams.
 * Fixed a bug with the "camera slow to load" message and increased the timeout.

## 1.9.22
### Released 10th November 2014
 * Hopefully fixing longstanding connection bug caused by bad interaction between iOS and cameras (specifically related to HTTP Keep-Alive and persistent connections).
 * Fixing some problems around behaviour on launch.
 * Now allows you to attempt to connect even if the device thinks it has no internet connection (to allow LAN connections).

## 1.9.21
### Released 3rd September 2014
 * Better handling of camera detection and falling back to more basic modes. Specifically this should work better with the newer Foscam firmwares.
 * Handling of infrequently updating cameras, e.g. public webcams. If app detects that the image is exactly the same on consecutive requests, it will back off and request the image less frequently.
 * Fixing “camera enters patrol mode on connect” error.
 * General bug fixes

## 1.9.20
### Released 20th December 2013
 * Initial support for audio on FI9821W, unfortunately there are currently problems with this on iOS6 and via a cell connection. See the [December2013](/december2013) page for more information on a temporary fix.
 * Also fixed a bug with the presets button on iPad.

## 1.9.19
### Released 23rd October 2013
 * Fixed problem with video feed flickering in landscape mode.
 * Fixed problem with named presets in iOS7

## 1.9.18
### Released 17th October 2013
 * Basic iOS7 UI support. 
 * Remembers app state between launches. 
 * More informative error messages.

## 1.9.17
### Released 18 September 2013
 * A quick update to fix the bug introduced in 1.9.16.
 * Also added another small fix to better support more cameras.

## 1.9.16
### Released 17 September 2013
 * **On initial upgrade you might find that the controls do not work at all. To fix this problem go to Settings on your device, then find "CamViewer" and set the "Force Config Download" option to "On" or "1".**
 * More consistent panning support and access to parameters after a complete overhaul of this and testing on over 250 cameras. 
  * This means more support for panning and for parameters such as brightness, contrast, etc. on many more makes and models of camera!
 * Support for accessing some cameras via SSL.
 * The ability to disable access via cellular connections.
 * URL support to enable you to link directly to cameras, see here for more instructions: [LinkingToApp](/linkingtoapp)
 * Fixed a timeout bug that cause connection to drop and reconnect after 30 seconds when audio is enabled.
 * Fixed various other bugs too.

## 1.9.15
### Released 19 April 2013
 * Improved talking support, attempt to improve listening support
 * Detects cameras that support the special 2-way audio api and falls back to using mjpeg feed on videostream.cgi for others.
 * Basic support for latest Foscam FI9821 cameras, just MJPG feed & controls so far.
 * Basic support for a few more cameras including iOS app IPCam, ABUS camera.
 * Fixed a bug with data usage not being recorded if the app went inactive.
 * Fixed a crash bug with preset popovers on iPad.
 * Fixed a bug that caused a 401 error on some cameras.
 * Fixing bug with aspect ratio breaking in proxy safer mode by completely changing "Proxy Safer" mode to work in a different way, also allows data usage to be displayed in this mode now.
 * Only shows "Controls disabled" message once.

## 1.9.14
### Released 25 January 2013
 * Fixes the bug that caused the app to disconnect when audio was enabled on some models of Tenvis camera.
 * Add basic support for the JPG feed from some H.264 cameras.
 * Stops warning about private networks if the user taps "Try anyway" and it works.
 * Attempts to reconnect to the feed if it disconnects.
 * General bug fixes and better detection of controls on more cameras.

## 1.9.13
### Released 10 January 2013

* Adds the ability to detect proxy servers and drop into "Proxy Safer" mode.
* Loads configuration from a web server allowing support for some new cameras to be added without having to release a new version of the app.
* Added support for presets on more cameras.
* Fixed a bug that stopped the app working on iOS 4.3.

## 1.9.11
### Released 28 December 2012

* Fixed the major bug that caused problems with lots of non-Foscam and Tenvis cameras.
* Added initial support for presets.
* Stopped showing the groups screen when the user didn't have any groups.

## 1.9.10 / 1.9.9
### Released 14 December 2012

A naming mismatch resulted in this version being referred to by two different versions at different times.

This version also unfortunately introduced a bug that caused the controls to not show up when using some brands of cameras.

* Introduced 2-way audio - the ability to send audio from the app to the camera.
* Added the ability for users to report problems from within the app. Gave the option of securely sending camera details to me making testing much easier.
* Added digital zoom, and optical zoom for cameras that support it.
* Added support for grouping cameras together.
* Added support for more types of camera.
* Better support for reverse proxy.
* Improved iPad layout when in landscape orientation.
* Hides nav bar and makes better use of available space.
* Unfortunately this version dropped support for devices running iOS less than 4.3.

## Pre 1.9.9
* Version 1.9.3 released 29 March 2012 introduced audio support, allowing users to listen to what the camera could hear.
* CamViewer for Foscam Webcams was originally released on 1st February 2011.
 * It was popular from the start even though it only provided basic video streaming and pan/tilt controls.
