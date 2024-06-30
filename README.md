# Nitro5-2018_AN515-52_OpenCore
My macOS Sonoma OpenCore EFI files and some others. Change SMBIOS serials if you are re-using.

```diff
- Update: Sold my Nitro 5 recently for an actual macBook upgrade so this will no longer be updated.
+ It was fun <3
```
![image](https://github.com/sameerasw/Nitro5-2018_AN515-52_OpenCore/assets/68902530/c68c9a17-360e-4220-8952-0997bcd89047)


## Specs:
| Component      | Description |
| ----------- | ----------- |
| Device      | Acer Nitro 5 (2018) AN515-52       |
| CPU   | Intel 8th Gen i7+ (I don't know why it's labeled with +) 8750H        |
| Chipset | Intel H370 (Coffee Lake) |
| RAM | DDR4 2666MHz 2x8GB |
| GPU | Nvidia GTX 1050 (Disabled in SSDT for lack of driver support in mac) |
| iGPU | Intel UHD Graphics 630 |
| Storage | ADATA Legend 710 256GB PCIe Gen3x4 m.2 SSD + 1TB Toshiba HDD @5600rps |
| Display | 15.6" FHD (1920x1080) LCD |
| Trackpad | l2C HID Synaptics |
| Wireless | Intel Wireless-AC AC9560 160MHz w/ Bluetooth |
| Ethernet | Realtek |
| Audio | Realtek ALC225 (Layout 30) |
| OS | macOS Sonoma 14.2.1 + Windows 11 23H2 |
| OpenCore | v1.0.0 |

## What Works?
- All USB Ports including Type-C
- Intel UHD 630 iGPU w/Graphics Accelaration
- Display w/backlight control
- WiFi + Bluetooth
- LAN
- Keyboard
- Keyboard Fn keys
- Trackpad
- Trackpad gestures
- m.2 and other SATA
- Audio (Speakers, Bluetooth Audio, 3.5mm port) + Mic
- Camera
- Battery capacity and indicator
- Device standby (Sleep) + Lid detection
- iMessage + Face time (w/Sonoma)
- USB Tethering
- Airdrop
- Screen Mirroring

## What's broken?
- Nvidia GTX1050 - Lack of driver support in mac
- HDMI - Connected to the dGPU

## Did not test
- SD card slot

## How to do it?
I have no idea. Tried for weeks and almost gave up, but finally figured out that it was the NVRAM that I didn't reset was causing boot issues for the OpenCore installer. It was done thanks to the mentioned guides, repos and personal support. This is my first hack build. Updated OC and all the kext files to their latest versions. Only problem is that my external audio sometimes add a hum sound when using 3.5mm port but since I use an USB audio adapter, it is ignored.

## Credits and ref
- [Thread on tonymacx86.com](https://www.tonymacx86.com/threads/guide-oc-monterey-acer-nitro-5-an515-52-core-i7-8750h-samsung-1tb-960-evo-pcie-nvme.319629/)
- [Dortanis's guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [pnapt's repo](https://github.com/pnapt/ACER-Nitro5-AN515-52-Opencore)
- [nerdynikhil's repo](https://github.com/nerdynikhil/Acer-Nitro-5-AN515-52-593F-OpenCore-Hackintosh)
- [duc010298-1's repo](https://github.com/duc010298-1/Acer-Nitro-5-AN515-52-Hackintosh-OC)
- [hanngoc1406's repo](https://github.com/hanngoc1406/Acer-Nitro-AN515-52-Hackintosh-OC-EFI)
- [acidanthera](https://github.com/acidanthera)
- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [r/hackintosh](https://www.reddit.com/r/hackintosh/)
- [To the members of my group](https://t.me/tidwib)

Enjoy! 
Keep hacking <3
