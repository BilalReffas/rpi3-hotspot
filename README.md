# rpi3-hotspot

Turns a Raspberry Pi 3 into a configurable access point.

## How this works

An access point is created if `/boot/hotspot.txt` file is present. If there is no such file, no access point will be set up and the `/etc/wpa_supplicant/wpa_supplicant.conf` will be used.

Defaults are `ssid=RpiAccessPoint` and `passphrase=rpiaccesspointpass` but can be changed by tweaking the `/boot/hotspot.txt` file. One or both parameters can be modified.  
The Raspberry Pi IP address will be `10.10.10.1`.

```
# /boot/hotspot.txt
ssid=RodrigoTheRobot
passphrase=thesecretpassphrase
```


## Installation

1. Clone this repo or download the archive.
2. `sudo ./install.sh`
3. Profit.
