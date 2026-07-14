# Klee Flashing Guide
Read carefully this guide if you want to flash any custom ROM made by @kylieeXD

## Requirements
----------------
1. vendor_boot.img
2. boot.img
3. lineage-23.3-xxxxxxxx-UNOFFICIAL-klee.zip

## Some Instructions
--------------------
1. Boot into bootloader use:
```
adb reboot bootloader
```

2. Flash vendor_boot use:
```
fastboot flash vendor_boot /path/to/vendor_boot.img
```

3. Flash boot use:
```
fastboot flash boot /path/to/boot.img
```

3. Reboot manually the device into recovery use:
```
fastboot reboot
```
After reboots, quickly hold volume up       button to boot into recovery

4. Formatting
```
Select Factory Reset -> Format Data
```

5. Enter to sideload
```
Select Apply Update -> Apply from ADB
```

6. Flash the ROM
```
adb sideload /path/to/lineage-23.3-xxxxxxxx-UNOFFICIAL-klee.zip
```
(or just drag and drop the zip file into terminal window after adb sideload command)

Notes:
- Choose yes after sideloading (reboots into recovery).
- ( Skip if you flash the GApps ROM. ) Flash GApps or magisk (optional, MindTheGapps recommended or anything u want).

7. Reboot to system
```
adb reboot
```
(or just Select reboot option on ur recovery)
