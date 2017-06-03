---
layout: page
title: December 2013 Update
---

> Please note that this was fixed a long time ago.

Unfortunately it looks like the support for the FI9821W has problems in some scenarios. It appears that it won't work with older versions of iOS and can have problems when connecting via cell or 3G connections.

I will put together a fix and release it as soon as possible. For now I recommend that you create a duplicate camera entry (Edit -> Duplicate -> Tap on the camera and edit the new camera's details) and set the Connection property to "Advanced Direct Image (No Audio)". You can then use this on iOS6 or when on a cell or 3G connection, and use the original when on Wi-Fi.

I understand that this is especially frustrating as the problems can occur when you have just paid for audio, I apologise for this. Please wait for an update but if you do ultimately want a refund you will need to contact Apple directly.

## Update 22nd December 2013

I have now tweaked the server so that any device not running iOS7 will get a modified config file and will not try to use the new code. This should stop the problem but will mean that for now you must be running iOS7 to be able to try the audio feature. I don't want to disable the new code completely as this will disable audio for people who have purchased it and for whom it may be working well.
