Target:
    Raspberry Pi 3B+

Date:
    2018/9/17

OpenWRT Version:
    [Latest OpenWRT commit:e51aa699f7ca3ce83a0add622c0fd17d0caafc46@master](https://github.com/openwrt/openwrt/tree/e51aa699f7ca3ce83a0add622c0fd17d0caafc46/)

Usage:
    1. Download the build root ([master.zip](https://github.com/openwrt/openwrt/archive/e51aa699f7ca3ce83a0add622c0fd17d0caafc46.zip)) or clone from the link above.
    2. Unzip build root, `./scripts/feeds update -a`, `./scripts/feeds install -a`
    3. Copy rpi3bp.config to the build root and rename it to .config
    4. `make -j8 V=99 | tee build.log`

Component:
    **ALL-IN-ONE** ( As many popular services/softwares as possible )
    But broken packages are simplely excluded.

Notice:
    1. Ethernet DHCP client failed: dhcp discovery sent by `udhcpc` via eth0 seems got no response. So no internet currently.
    2. The other functions are working well.
