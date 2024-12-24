### Pre-installation:

* Gapps: [NikGapps](https://nikgapps.com/downloads) or [crGapps](https://nikgapps.com/crdroid-official)
* Optional: [KernelSU](https://github.com/tiann/KernelSU)
* TWRP and Boot: [Download](https://sourceforge.net/projects/crdroid/files/haydn/11.x/boot/) (Download any one depending how you want to install)

### Installing TWRP

* You need to have [Platform Tools](https://developer.android.com/tools/releases/platform-tools) in your PC (Navigate to ***"Download SDK Platform-Tools for Windows"***)
* Now go to Downloads and unzip it. 
* Open the folder and search

```
cmd
```
* It will open the command terminal
* Now on the phone hold the ***POWER + VOLUME Down*** together for 5-10 seconds until the phone enters the Fastboot Mode
* Now type

```
fasboot devices
```
* Your device will be shown in the terminal as a fastboot device
* Now type

```
fastboot boot [drag-and-drop-the-twrp-image-in-termnal]
```
* Now you are booted to TWRP

### Fisrt time installation

* ### Installing via TWRP
* ***Note: Please go through the Installing TWRP once***
* Backup your data to PC, OTG flash drive.
* Open the platform tools in PC
* Type

```
cmd
```
* Hold the power and volume up buttons together for 5-10 seconds until it boot to TWRP
* Now navigate to ***WIPE > ADVANCE WIPE***
* Select: ***data, metadata, cache, dalvik cache***
* After wiping go back and navigate to ***Install***
* Select the crDroid zip and the gapps (if any)
* After the flash is done, simply reboot
* Enjoy !!!

### Installing via crDroid recovery
* Firtly, boot to fastboot
* On PC terminal type

```
fastboot boot [drag-and-drop-the-twrp-image-in-termnal]
```
* Now in recovery go to factory reset and confirm the reset
* Reboot to recovery
* Choose apply update and Apply from ADB
* Now install crDroid zip via sideload with

```
adb sideload [drag-and-drop-the-zip-in-terminal]
```
* Reboot to recovery
* Flash gapps with

```
adb sideload [drag-and-drop-the-gapps-in-terminal]
```
* Reboot and enjoy !!!

### Update installation:

### 1. Using TWRP
* Boot to TWRP Recovery (Hold Pow + Vol Up)
* Download the the update zip in the storage of the device
* Choose install 
* Select the crDroid.zip and gapps (if the phone has gapps before update)
* Reboot and enjoy !!!

### 2. Using crDroid recovery
* Boot to crDroid recovery (Hold Pow + Vol Up)
* Open Terminal in your pc (in the the platform tools folder)
* Type:

```
adb devices
```
* It will show your and device code and mode type
* Now head to the recovery: ***Apply Update > Update Via ADB***
* Now type (in terminal):

```
adb sideload [drag-and-drop-in-terminal-cr.zip]
```
* Flash gapps

```
adb sideload [drag-and-drop-in-terminal-gapps.zip]
```
* Reboot and enjoy !!!

### 3. Update via OTA
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* If having gapps, reboot to recovery and sideload gapps package again
* Reboot
