---
layout: page
title: Known Issues
---

There are a few issues with the app that I know about but haven't been able to fix yet. I'll probably forget to list some but I thought I'd start a list so that I have somewhere to put them for now. Hopefully this list will get shorter as time goes by :-)

 * **Cameras No Longer Connecting** - If the updates around September 2014 have caused problems for you it's most likely due to the new support for audio on more HD cameras. If you have a HD camera you might find you need to enter the media or RTSP port value for your camera. You will also need to be forwarding that port from your network. An alternative is to modify the Connection property to "Advanced Direct Image" which will disable the audio support.
 * **Audio Problems** - The audio quality isn't amazing with these cameras but there is still some work I can do to improve it. In particular sending audio from the app to the camera varies in quality a lot.
 * **Controls Problems** - The app was only built originally to support a single type of Foscam camera but actually supports many cameras by many manufacturers. Unfortunately some cameras have slight differences leading to pan controls working in the opposite direction or preset or other buttons not showing up. If you can report this from within the app, and ideally send me the camera's ip address I will look into these and try to support more with each version.
 * **HD Video Problems** - I'm aware of an issue with the HD video feed appearing corrupted. This may be a bandwidth issue so you may like to try reducing the quality of the feed but I'm looking into the issue further. I have found that setting one of the streams to 720P/200K/25FPS/25 and telling the app to connect to that stream works well  (do this in Settings -> Video -> Video Settings on your camera).

## Fixed Issues
 * **HD Video Crash** - ~~Newer RTSP style cameras cause an app crash occasionally.~~ Fixed in [1.9.26](/changelog#1926)
 * **Disconnect Problems** - ~~It seems the app disconnects from the camera feed when it shouldn't. Sometimes this may simply be a network problem but it does seem to happen more with CamViewer than with other apps or the web feed. I will look into what's causing the problems but will also put an auto-reconnect feature in too.~~ Hopefully fixed in version [1.9.22](/changelog#1922), I haven't had so many reports since.
 * **Camera pans when you first connect to it** - ~~I know what's causing this problem but unfortunately it will mean changing how I'm dealing with the controls so it's not a quick fix, it's definitely on my list though.~~ This was fixed in version [1.9.21](/changelog#1921)
 * **Foscam Connection Problems** - ~~Later Foscam firmwares have broken the ability for CamViewer to detect the special API that they provide. You can force CamViewer to use this by editing the camera and setting the Connection property to **Special 2-way Audio API**~~ Version [1.9.21](/changelog#1921) handles this better by trying this first and giving you the option to fall back to a  more basic mode if the feed is taking a long time to load.
 * **Audio Disconnect Problem** - ~~The app has problems with some cameras, notably a model made by Tenvis, and will disconnect from the camera as soon as you turn on audio support. This will be fixed as soon as possible.~~ This was fixed in version [1.9.14](/changelog#1914).
 * **Controls problem with v1.9.16** - Updating to [v1.9.16](/changelog#1916) can cause your controls to stop showing up. This should fix itself within 24 hours of you upgrading but you can force it to happen sooner by going to Settings on your device, then find "CamViewer" and set the "Force Config Download" option to "On" or "1".
 * **Connection Problem with v1.9.14** - Updating to [v1.9.14](/changelog#1914) causes the app to stop connecting to any cameras. Rebooting iOS your device (i.e. turn it off completely and turn it back on) appears to fix this problem.
 * **Wanscam JW0004** - Should work if you set Connection to "Proxy Safer" mode and also give it the index.htm filename, i.e. http://example.com/index.htm will work, http://example.com/ will not work until the next update.
