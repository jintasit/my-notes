## Linux mint has suspend issue with my bluetooth dongle
[Link](https://forums.linuxmint.com/viewtopic.php?t=408260)

## Logitech MX 3 middle mouse's wheel doesn't working on Firefox after suspended
I faced this issue in many linux destros for example Ubuntu, Mint, Fedora. All of them has same problem with Logitech MX3 mouse.
[Link](https://askubuntu.com/questions/1163408/why-does-my-mouses-scroll-wheel-stop-working-after-resuming-from-suspend-in-xub)

Following bash script I used with Fedora destro.

```bash
#!/bin/bash

if [[ $1 == post ]]; then
	rmmod hid_logitech_dj
	modprobe hid_logitech_dj
fi

```
