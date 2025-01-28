![Remote Play dialog](images/remote-play.png){ width="400" }

## Features
- Allow you to use Remote Play in the browser.
- Support streaming Xbox 360 games with 1080p resolution.
- Can play even when you're not using home network.

## Set up Remote Play on Xbox

1. Setup static IP address on the console:
    - Settings > Network settings > Advanced settings
    - Note down IP address, Subnet Mask, Gateway, and DNS values
    - Click on IP settings > Static > enter the values you noted in previous step
    - Save

2. Follow this [official guide](https://support.xbox.com/en-US/help/games-apps/game-setup-and-play/how-to-set-up-remote-play) to enable the Remote Play feature on your Xbox.  

3. Setup [port-forwarding](https://support.xbox.com/en-US/help/hardware-network/connect-network/network-ports-used-xbox-live) on your network.  

4. Make sure your Xbox have "Open NAT" status.  

!!! note
    To use Remote Play when not using the network as the console, open these additional ports (both TCP & UDP, just in case):  

    - 4838
    - 5050
    - **9002** (this one is a must)
    - 50302

    Another options: do one of these methods if your router supports it  
    
    - Enable IPv6
    - Setup [Tailscale](https://tailscale.com/)

    If it still doesn't work, check with your internet provider.  
    These is nothing else I can help. It's not a bug, don't report it. 

## Enable the Remote Play feature in Better xCloud
1. Open Better xCloud's settings.
2. Check the "Enable Remote Play feature" checkbox.
3. Reload the page.
4. Now you'll see the "Remote Play" button next to your profile picture.
