---
layout: page
title: Test In-App Purchases
---

I'm trying to send out test versions of the app to a bunch of people before submitting to the app store. I'm using a system called TestFlight which makes installing the test versions a breeze. The test version will install separately to your main version so if there's any bugs in the test version, they shouldn't affect your use of the main app. The test version shows up on your device as CamViewer β

Because this will show up as a separate app it won't have your list of cameras. [The app has an import/export feature](/exporting-and-importing) that you can use if you want to export them from your main app and import them into the test version. Alternatively just add a new camera entry manually.


If you want to test the audio features you will obviously need to purchase this. With a test build you can't actually use your own app store details to buy in-app purchases, you will need to use a test account. Here's how:

 * Before installing go into Settings, find Store, tap on your Apple ID and then tap "Sign Out" (it's probably not so important that you do this before installing the app but if you're having problems, try deleting the app and start from the beginning again).
 * Install the app using TestFlight
 * Start viewing a web cam with your device portrait, you should see a speaker icon (on the iPhone it shows on the right, on the iPad on the left, Audio is not supported on older devices such as the iPhone 3G so will not show up on these devices)
 * Tap on the speaker icon, a list will come up showing the available in-app purchases, currently only Audio support.
 * Tap on the price and then tap to buy, you will be asked to sign into the Store, sign in using one of the test accounts listed below.
 * When asked, confirm that you would like to purchase the feature.
 * Purchase should complete, a confirmation should show and you will be returned to the camera view.
 * The audio option should already be selected but if not, tap the speaker icon again.
 * You should now have audio!

## Test Accounts

It's a while since I've used these test accounts and I'm not entirely sure that it is actually possible to share them with multiple users. Try the details below, if you're having problems then let me know and I'll create an account just for you.

| Username | Password | App Store Country | |
| --- | --- | --- | --- |
| cv-uk@mckerrell.net | 1Qwertyuiop | UK |
| cv-us@mckerrell.net | 1Qwertyuiop | US |
| cv-nl@mckerrell.net | 1Qwertyuiop | Netherlands |
| camviewer-gb2@mckerrell.net | 1Qwertyuiop | UK |
| camviewer-gb3@mckerrell.net | 1Qwertyuiop | UK |
| camviewer-nl@mckerrell.net | 1Qwertyuiop | Netherlands |
| ~~cv@mckerrell.net~~ | ~~1Qwertyuiop~~ | ~~UK~~ | Disabled |