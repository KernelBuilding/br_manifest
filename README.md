<p align="center">
 <img src="https://raw.githubusercontent.com/BatikRecovery/br_manifest/android-9.0/batik-recovery.png" > 
</p>

<div align="center">
<a href="#">
  <img src="https://img.shields.io/badge/platform-android-blue.svg?style=flat-square"
    alt="platform" />
</a>

<a href="#">
  <img src="https://img.shields.io/badge/build-unstable-brightgreen.svg?style=flat-square"
    alt="build" />
</a>

<a href="#">
  <img src="https://img.shields.io/badge/version-B 1.6.0-green.svg?style=flat-square"
    alt="version">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/base-twrp 3.7.1-orange.svg?style=flat-square"
    alt="base">
</a>

</a>
<a href="#">
  <img src="https://img.shields.io/badge/license-apache%202.0-3F51B5.svg?style=flat-square"
    alt="base">
</a>

</div>

Overview
=======

Batik Recovery is Project Recovery developed by Batik Recovery Teamwork from Indonesia, this Batik Recovery is a derivative of the Official TWRP that was modified by the developer in accordance with the Indonesian characteristics. In Indonesia, batik is a motif that is considered quite famous for the beauty of its art. Therefore, the developer gave the name Batik Recovery and a touch of batik motifs in the Recovery, including splash, background, and icon. The goal of the developer to release the project is to further popularize batik, and especially to popularize the name of Indonesia.

Features
=======

* Support Treble (Vendor) or Non Treble
* Support GSI, Android Pie
* Support Miui OTA
* Support F2fs
* Ramdisk Cleaner
* Enable / Disable HAL3
* App Delete
* Enable / Disable Navbar
* Del Subs Overlay
* Lazy Flasher
* Reset Password
* Aroma FM
* Root / Unroot Magisk
* Mount Magisk
    
Changelog
=======    

~ Alpha-01 ~
* Initial Build

~ Alpha-02 ~
* Add Fitured

~ B v1.1 ~
* Upstreamed base TWRP 3.2.3-0
* Update Batik Theme v1.1
* Update Magisk 16.71
* Add Indonesia, Sunda Language
 
~ B 1.2 ~
* Overlay Reboot Menu
* Add some icon style
* Update Magisk 17.1
* Add Jowo Language
* Full Backup / Restore Partition
* Further ensure TWRP is not replaced by stock recovery
 
~ B 1.3 ~			
* Add Square Style, Circle Style Icon
* Add Change Color Theme (Header & Navbar)
* Change Themes without Reboot
* Update Magisk 17.2
* Add Mount Magisk (Tools)
* Merge September Security Patch (android-8.1.0_r46)	

~ S 1.4 ~
Changelog Xiaomi :
* Add Wipe Substratum on Page Wipe
* Add Automatic Disable DM-Verity
* Add OTA MIUI Support
* Update Magisk 17.3
* Update October Security Patch

Changelog Asus :
* Add Wipe Substratum on Page Wipe
* Update Kernel
* Update Magisk 17.3
* Fix Overlay on Menu Reboot
* Merge October Security Patch (android-8.1.0_r47)

~ S 1.4.1 ~
* Update Theme
* Add Regional language in Indonesia
* Add Russian, Malay, Turkish, Vietnamese, Portuguese, Japanese Language

~ S 1.4.2 ~
* Fix Bug Progress Bar

~ S 1.4.5 ~
* Update Februari Security Patch (android-8.1.0_r61)
* New Brand Logo
* New Splash with New Brand Logo
* Update Flashable Camera2API Compatible with Oreo/Pie
* Update DFE and DM-Verity in Source Batik
* Update Flashable Magisk Stable 18.1
* Add Tools : Adblock, MIUI OTA disabler and Asus Decrypt

~ S 1.5.0 ~
* Upstremed Base TWRP 3.3.1-0
* Remove MIUI OTA SUPPORT
* Update June Security Patch (android-8.1.0_r65)
* Whyred, kenzo, rolex, riva : Update Device Tree base android-9.0
* Whyred, kenzo, rolex, riva : Update July Security Patch (android-9.0_r45)
* Delete Mount Magisk, change Magisk Manager for Recovery
* Update Flashable Magisk Stable 19.3

~ S 1.6.0 ~
* Upstremed Base TWRP 3.7.1-12.1

Credits
=======
* [**TEAMWIN RECOVERY PROJECT (BASE)**](https://github.com/TeamWin)
* [**OMNIROM**](https://github.com/omnirom)
* [**REDWOLF RECOVERY PROJECT**](https://github.com/RedWolfRecovery)
* [**PITCHBLACK RECOVERY PROJECT**](https://github.com/PitchBlack-Recovery)
* [**DARK RECOVERY PROJECT**](https://github.com/DarkRecovery)
* [**ORANGEFOX RECOVERY PROJECT**](https://gitlab.com/OrangeFox)

Donation To Zhantech
=======
* ZHAN Project Paypal - http://paypal.me/zhantech
* ZHAN Project Tester and Report - http://t.me/ZHANreport
* ZHAN Project Instagram - https://www.instagram.com/zhantech
* ZHAN Project Facebook - https://m.facebook.com/zhantech

Getting Started
===============

### script for download all packages

```bash
cd ~ && sudo apt install git -y && git clone https://github.com/akhilnarang/scripts && cd scripts && sudo bash setup/android_build_env.sh && sudo bash setup/install_android_sdk.bash
```

### create directory

```bash
mkdir batik
cd batik
```

### initialize Batik Recovery local repository, use this command :
```bash
repo init -u https://github.com/KernelBuilding/br_manifest.git -b android-12.1
repo sync -j$(nproc --all)
```

 Compilation Of Batik Recovery
=============================
 
```bash
cd batik
export ALLOW_MISSING_DEPENDENCIES=true
export BR_MAINTAINER="your-name"
```     
 
```bash
source build/envsetup.sh
lunch twrp_<device>-eng
mka recoveryimage
```
