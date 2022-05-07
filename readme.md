# Samsung Galaxy F22 4G SM-E225F / DS 
# TWRP Device Tree

TWRP Device tree for the Samsung Galaxy F22 4G MediaTek

This tree compatible with TWRP 3.6.11 as of 30/04/2022

---
![Samsung Galaxy F22 4G](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-f22-1.jpg)


# About Device

Samsung Galaxy F22 4G MediaTek (f22)

### Specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 6x1.8GHz Cortex-A55 + 2x2.0Ghz Cortex-A75, ARM big.LITTLE
Chipset | MediaTek Helio G80 (mt6769t)
GPU     | ARM Mali-G52 MC2
Memory  | 4 GB / 6 GB
Shipped Android Version | OneUI 3.1 on top of Android 11.0
Updated Android Version | N/A
Storage | 64 GB / 128 GB
MicroSD | Up to 256 GB
Battery | 6000 mAh (non-removable) (SM-E225F / DS)
Dimensions | 160 x 74 x 9.4 mm (6.30 x 2.91 x 0.37 in)
Display | 720 x 1600 pixels, 6.4" Super AMOLED
Rear Camera  | 48 MP, f/1.8, (wide), PDAF, 8 MP, f/2.2, 123˚ (ultrawide), 1/4.0", 1.12µm, 2 MP, f/2.4, (macro), 2 MP, f/2.4, (depth), LED Flash
Front Camera | 13 MP, f/2.2, (wide)

---

#  Steps to Compile

 Place the device tree in proper location $SOURCE_HOME/device/samsung/f22/ 
 
 Add AOSP TWRP Source or Minimal TWRP Source
 
 `repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11`
 
Then Run `repo sync` 

```sh
. source ./build/envsetup.sh && lunch twrp_f22-eng && make clean && make -j# recoveryimage
```
`# = No. of CPU threads of your PC'

#  Kernel Source here

 Kernel Source from which the prebuilt kernel is included in tree under prebuilt directory.
 
 Will be added shortly.

### Thanks to:
 * Me, akhil1999
 * TeamWin
 * @sunmughan for testing.

