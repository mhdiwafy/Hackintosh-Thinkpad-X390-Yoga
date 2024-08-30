# Hackintosh-Thinkpad-X390-Yoga

**❗️❗️DISCLAIMER❗️❗️**<br>
Read the entire README before you start.
The developers are not responsible for any damages you may cause.
Should you find an error or improve anything — whether in the config or in the documentation — please consider opening an issue or pull request.

<details>  
<summary><strong>Table of Content 📖</strong></summary>
</br>

## Table of Content📖
- [Hackintosh-Thinkpad-X390-Yoga](#Hackintosh-Thinkpad-X390-Yoga)
- [Table of Content](#Table-of-Content)
- [Device Information](#Device-Information)
- [Whats working](#Whats-working)
    - [CPU](#cpu)

</details>

## Introduction✨

<details>  
<summary><strong>Device Information💻</strong></summary>
</br>

## Device Information
| Specifications | Details |
|:---|:---|
| Computer Model | ThinkPad X390 Yoga |
| CPU | Intel(R) Core(TM) i5-8265U CPU @ 1.60GHz |
| Model |  Lenevo 20NQ|
| Display | Lenevo LEN4094 ( 13.3 inch  ) Touchscreen |
| Memory | 16 GB ( Soledered, SK Hynix DDR4 2400 MHz ) |
| NVMe SSD | NVME Micron 2450 512  GB |
| Integrated Graphics | Intel UHD Graphics 620 |
| Ethernet |  Intel(R) Ethernet Connection (6) I219-V |
| Sound Card | Intel Intel Smart Sound Technology Audio Controller (layout-id: 11) |
| Wireless Card |  Intel(R) Wireless-AC 9560 160MHz |
| I/O |1xUSB-C Thunderbolt 3, 1xUSB 3.1 gen 1(type-c), 2xUSB 3.1 gen 1, MicroSD card reader, HDMI 1.4, 3.5mm Headphone jack/mic combo |

</details>

<details>
<summary><strong>Whats working</strong></summary>
</br>

## Whats Working

### CPU

Work fine, thanks to `CPU friend and CPU FriendFriend`, Patched to 0.8 Ghz (Min) - 2.4 Ghz (Max)
Using CPU Friend data provider on lowest power consumsion.
For me, no serious Performance Effect on this setting<br>
Great for Daily usage, such as office, sone video editing, graphic design, some multitask, of course browsing.<br>
on the efi, i insert the `Performance profile` as default<br>
if you want to change the power setting,<br>
i will give the further assistance on the "other tweaks" section

### Battery 

The battery presentage is function normally

### USB

USB Ports Patching with `USBMap.kext` , everything works fine, no serious issue with USB

### Ethernet

Functioning normally. thanks to `IntelMausi.kext`

### Display

The model of Integrated Graphics is `Intel UHD Graphics 620`, faked to `Intel UHD Graphics 630 (Mobile) `.

The HDMI is attached with `Intel UHD Graphics 630` and it's functioning normally. `2K@60Hz` & `4K@30Hz` are supported.

Both USB-C is also work as Display Out (like HDMI), which utilize Display Port(DP) function, You can use it as another option for display out, you might need a supported dongle or supported Type-C cable 

### Audio
thanks to AppleALC with `layout-id: 11`. works normally. Support Dolby Audio.

### Keyboard

Functioning normally except the <kbd>Insert</kbd> , which is not presented on Magic Keyboard.

#### SSD

NVMe is functioning normally.

### Bluetooth

Bluetooth functioning partially<br>
There is some issue if you use `Airportitlwm.kext` as the wifi kext
but if you are using `itlwm.kext and Heliport.app` it will no issue

### Wireless-Card

Functioning normally. <br>
if you are using `Airportitlwm.kext`, it will cause an issue, the wifi speed will drops whenever connected to the bluetooth device, and hard to connect BT device when you are connected to 2.4Ghz Wi-Fi<br>
highly recommend for you to use `itlwm.kext and Heliport.app`

### Headphone/mic combo

Functioning normally. if you facing trouble please read `post install`

### Other

#### AirPlay
working on sonoma, but somehow not working on ventura
#### Handoff
same `apple id` is required

## What-is-not-working

- Continuity Camera fail to work properly, but Handoff works, and Airdrops can achieve one-way transmission from computer to iphone

</details>