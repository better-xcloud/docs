---
title: How to tweak Android WebView for better performance
---

# How to tweak Android WebView for better performance

> [Why does the performance suck on Android TV?](../faq.md#android-app)

!!! note
    - You don't need to follow this guide if your device can play xCloud without any problem!
    - This guide is recommended for Android TV devices

## Steps to setup

Follow this guide to improve the performance of Android WebView inside the Better xCloud app and make it useable.

!!! info
    This guide has been tested on these devices:  

    - ✅ Working:  
        - Chromecast with Google TV 4k: `720p/High`  
        - Xiaomi TV Box 4k 2nd gen: `1080p/High`  
        - onn. Google TV 4K Streaming Box (2023): `1080p/High`  
    - ❌ Not working:  
        - Most, if not all TCL TVs

    If your device isn't in the list above, try to follow the guide and report back the result. Thanks.

1. Install [Android app](https://github.com/redphx/better-xcloud-android/releases/latest)  

2. Open the **Better xCloud** app, then go to the App settings

3. Enable `Optimize WebView performance` setting  
> ??? info  
>     This will automatically set these flags in the WebView:  
>
>     - ignore-gpu-blocklist: `✅ Enabled`
>     - WebViewThreadSafeMedia: `✅ Enabled`
>     - WebViewSurfaceControl: `✅ Enabled`
>     - WebViewSurfaceControlForTV: `✅ Enabled`
>     - WebRtcCombinedNetworkAndWorkerThread: `❌ Disabled`  

4. Open `WebView Manager > Downloader`, then download and install any of these WebViews:
    - Thorium WebView: best WebView if your device supports it
    - Mulch WebView

5. After installing, switch back to the `Installed` tab, press `Refresh`, then select the recently installed WebView.

6. Close the Settings screen, force close Better xCloud app, then re-open it.

7. Set these Better xCloud script's settings:  
    - Disable xCloud analytics: `Enable`
    - User-Agent: `Android TV`
   
    Save and reload the site

8. Done. Now you can play a game and see the result.

9. If it's still unplayable:  
    - Open Stream settings, try changing Video's renderer to `WebGL2`. There are reports that doing this makes it playable on TCL TVs.  
    - Try [Edge Browser](../android-browser.md)
    - Buy a better device
