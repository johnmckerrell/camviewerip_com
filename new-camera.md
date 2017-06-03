---
layout: page
title: New Camera
---

How to add a new camera.

1. Add an entry to pathMunges
  * matchRegex - if this matches the response string for the URL entered by the user, then this path munge is used.
  * stripRegex - this regex is applied to the URL to strip it back to a base URL. 
  * mungeFormat - this builds out the URL to retrieve an image to display and can have the following components
    * %@ - the base URL calculated by applying stripRegex.
    * !!USERNAME!! - the username entered by the user in the config.
    * !!PASSWORD!! - the password entered by the user in the config.
2. Add the filename to filenameMatchRegex, make sure you include any query string parameters that may occur (or .*)
  * Add the query parameters bit to matchedFilenameStrippingRegex so that it gets stripped down to a basic filename
  * The filename will now be used as a controls filename, so you probably want to put a match into cameraControlFilenameAlternatives to convert the image filename into a controls filename.
3. Add to matchControlsRegex something that will match the content of the page you've just added as a controls file.
4. If necessary add a new set of values to cameraProperties
5. Add an entry to cameraPickerRegexes to match the right camera and do something useful with it.