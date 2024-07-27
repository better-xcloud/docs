---
title: How to tweak Android WebView for better performance
---

# How to tweak Android WebView for better performance

> [Why does the performance suck on Android TV?](../faq.md#android-app)

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

## Steps to setup:
1. Install [Android app](https://github.com/redphx/better-xcloud-android/releases/latest)  

2. Install [Thorium WebView](https://thorium.rocks/):
    - 64-bit device: [SystemWebView_arm64.apk](https://github.com/Alex313031/Thorium-Android/releases/download/M124.0.6367.218/SystemWebView_arm64.apk)  
    - 32-bit device: [SystemWebView_arm32.apk](https://github.com/Alex313031/Thorium-Android/releases/download/M124.0.6367.218/SystemWebView_arm32.apk)  

    > If you can't install the app, ensure there are no apps on your device with `com.android.webview` as package name. If there is one, uninstall it and try again if it's not a System app.  
    > Otherwise you can continue with the guide using the default System  WebView, but don't expect the same result.

3. Open the **Better xCloud** app, then go to the App settings

4. Enable `Force low-latency audio`

5. Change `WebView implementation` to `Android System WebView 124.0.6367.218` (this one is Thorium WebView)

6. Open `WebView DevTools`, then select the `Android System WebView` with the blue globe icon > `Just once`.

7. Inside `WebView DevTools` screen, switch to `Flags` tab, then change these flags to:
    - ignore-gpu-blocklist: `✅ Enabled`
    - WebViewSurfaceControl: `✅ Enabled`
    - WebViewThreadSafeMedia: `✅ Enabled`
    - VSyncDecoding: `✅ Enabled`
    - BackgroundResourceFetch: `✅ Enabled`
    - ThreadPoolCap2: `❌ Disabled`
    - WebRtcCombinedNetworkAndWorkerThread: `❌ Disabled`  

    *(some of these flags may be not neccessary)*

8. Force close Better xCloud app, then re-open it.

9. Set these Better xCloud script's settings:  
    - Disable xCloud analytics: `Enable`
    - User-Agent: `Meta Quest VR`
   
    Save and reload the site

10. Done. Now you can play a game and see the result.

11. If it's still unplayable:  
    - Open Stream settings, try changing Video's renderer to `WebGL2`. There are reports that doing this makes it playable on TCL TVs.  
    - Try [Kiwi Browser](../kiwi-browser.md)
    - Buy a better device
