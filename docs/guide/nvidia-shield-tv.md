
### Some buttons (Select/Guide/...) on the controller not working

This was caused by a system modification by NVIDIA that remaps some controller buttons on a system level. You can fix this issue by disabling or uninstalling the `com.nvidia.shieldtech.hooks` package.

Two ways to do this:  

- Via ADB command: `adb shell pm disable-user com.nvidia.shieldtech.hooks`  
- Use the [ADB TV: App Manager](https://play.google.com/store/apps/details?id=com.cybercat.adbappcontrol.tv) app, find the package and disable it  

After that restart the NVIDIA Shield TV.
