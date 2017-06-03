---
layout: page
title: RTSP Support
---

CamViewer has RTSP support for some cameras. On the Foscam FI9821W this support will be picked up automatically and used. If you know that your camera supports RTSP but CamViewer isn't detecting it, you can link directly to the RTSP URL by entering 

`rtsp://username:password@hostname:port/path`

For now you must enter the username and password both in the URL and in the relevant fields in CamViewer, I hope to improve on this later. Also you will find that any PTZ features offered by your camera won't work (although the app will often try to do a safe fallback to basic Foscam controls so you might still see PTZ controls). If you want full support for a new camera let me know and I'll try to add it although I really need access to a camera to add support for it.