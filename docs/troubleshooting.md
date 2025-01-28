## I got the "Failed to run Better xCloud" error message

!!! note "Chrome/Edge/Chromium"
    *⚠️ This is Tampermonkey's problem. Don't report it on Better xCloud GitHub.*  

    For users of the Tampermonkey extension in a Chrome-based browser, enabling `Developer Mode` is a requirement introduced with Manifest V3 updates.
    
    1. Check Tampermonkey's dashboard to make sure you installed the script correctly
    2. Open the browser's Extensions page
    3. On the top right corner, click the `Developer Mode` toggle to enable it
    4. Reload xCloud website

    If it still doesn't work, do these additional steps in Tampermonkey's Settings page:  

    1. `General` > `Config mode` > `Advanced`
    2. `Security` > `Content Script API` > `UserScript API Dynamic`
    3. (Optional) `Experimental` > `Inject Mode` > `Instant`
    4. Reload xCloud website
