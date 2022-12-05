# Networking

I love both networking hardware and software.  Firmware, protocols, appliances, I collect it all.

## OpenWRT

[OpenWRT](https://openwrt.org/) is probably my favorite networking firmware.  Awesome packages which can turn relatively simple pieces of equipment into very complex routing platforms.

The below devices I have either successfully installed OpenWRT, partially succeeded in installing OpenWRT or really wish I could install OpenWRT.

## MikroTik RB5009

Love the [MikroTik RB5009](https://mikrotik.com/product/rb5009upr_s_in).  This is a great piece of hardare, PoE+ ports with cycles to spare but unfortunately OpenWRT isn't *quite* compatible but that seems [to be changing](https://github.com/Arie/openwrt-rb5009)


## MikroTik hEX S

The [MikroTik hEX S](https://mikrotik.com/product/hex_s) Works flawlessly with OpenWRT and has hardware flow offloading.


## Ubiquiti Access Point U6 Long-Range
At one point I was very much into Ubiquiti and their UniFi series such as the [Ubiquiti Access Point U6 Long-Range](https://store.ui.com/products/u6-lr-us) but their firmware leaves a lot to be desired.

I was able to successfully flash the UniFi 6 with OpenWRT but would reboot during high load and was unstable when you needed it most.


## Netgate SG-3100
The [Netgate SG-3100](http://www.netgate.com/blog/introducing-sg-3100-appliance) was a fantastic piece of hardware but being ARM meant not every package they offered would work on the platform (looking at you Telegraf)

While the pfSense interface is very powerful, I still prefer command line and being unable to flash the device to another firmware is just a bummer.
