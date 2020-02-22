# Example wpa_supplicant.conf
Paste this into your `wpa_supplicant.conf` file that you put into the `boot` folder on the micro sd card of your Pi.
Make sure you set your correct country code as listed at: https://en.wikipedia.org/wiki/ISO_3166-1

```
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=<Insert country code here>

network={
 ssid="<Name of your WiFi>"
 psk="<Password for your WiFi>"
}
```

This info comes from the official Raspberry Pi documentation found here: https://www.raspberrypi.org/documentation/configuration/wireless/headless.md
