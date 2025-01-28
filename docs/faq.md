## General

1. **Will I get banned for using this?**  
> xCloud devs endorsed Better xCloud before and confirmed they ["don't ban people for using a third party client or extension"](https://old.reddit.com/r/xcloud/comments/1b5d4dl/new_better_xcloud_feature_play_local_coop_games/kt6w1wt/). As always, use it as your own risk.

2. **Why is it an Userscript and not an extension?**  
> It's because not many browsers on Android/iOS support installing extensions (and not all extensions can be installed).

3. **Why doesn't the xCloud website implement *this* or *that* feature from Better xCloud?**  
> Think of this project as an unofficial beta version of xCloud.  
>     - **Better xCloud** doesn't have to worry about the compatibility much: if it doesn't work on this browser, it can just suggest you switch to another one. xCloud can't do the same.  
>     - On the xCloud's side, they have a lot more users and devices to support, so it's more difficult for them to implement a new feature.  
>     - Also, it's not easy to explain some of the features of **Better xCloud** to normal xCloud users.  

4. **Can I use this with the Xbox Android app?**  
> No, you can't. You'll have to modify the app.

5. **Will it be able to request a lower FPS or increase the maximum bitrate (15Mbps) of the stream?**  
> Sorry, no. The server decides all these settings.

6. **Other apps can set minimum and maximum bitrate, why Better xCloud can't?**  
> Those settings are useless, they don't do anything except for the maximum bitrate feature, but it works when the value is less than 15MB/s. That's why in **Better xCloud** you can only limit the bitrate value up to 14MB/s.

## Android app

1. **xCloud works in the Xbox Game Pass app but not the Better xCloud app...**  
> The Xbox Game Pass app is a native app, meanwhile Better xCloud app is a WebView wrapper of the xbox.com/play website, so it's expected to have slightly worse performance. Also the Xbox Game Pass app only has 720p video resolution.

2. **The video is flickering on my Android TV...**  
> Most Android TVs use cheap hardware, so don't expect the app will work. Check answers below for workarounds.  

3. **Some games work, some don't**  
> Your device is struggling against high framerate games or high bitrate scenes. And no, I can't lock framerate at 30 FPS.  

4. **Settings & Refresh buttons on the bottom right of Android TV app can't be clicked...**  
> The app is not optimized for Android TV, both UI and performance. You'll need an air-mouse or bluetooth mouse to interact with the UI.

5. **Will there be a native app for Android or Android TV?**  
> No, it will take a lot of time, so I don't plan to.  

6. **Why can I play normally with Edge Browser but not with the Better xCloud app?**  
> Edge Browser uses *Chrome rendering model*, meanwhile Better xCloud app uses *WebView rendering model*, and this one has worse performance due to the way it was designed. Read more about it [here](https://issues.chromium.org/issues/40817676#comment65).

7. **Anything I can do do improve the performance?**  
> - Follow [this guide](guide/android-webview-tweaks.md) to tweak the performance.  
> - Limit maximum bitrate.  
> - Lower resolution + visual quality.  
> - Switch to Edge Browser.  
>
> If none of these method works then there is no help. Buy a better device.
