# Klee Flashing Guide (OrangeFox)
Read carefully this guide if you want to flash any custom ROM made by @kylieeXD

## Requirements
----------------
1. OrangeFox-R12.0-Unofficial-klee-system-compatible.img
2. lineage-24.0-xxxxxxxx-UNOFFICIAL-klee.zip

## Some Instructions
--------------------
1. Boot into bootloader use:
```
adb reboot bootloader
```

2. Flash vendor_boot use:
```
fastboot flash vendor_boot /path/to/OrangeFox-R12.0-Unofficial-klee-system-compatible.img
```

3. Reboot manually the device into recovery use:
```
fastboot reboot recovery
```

4. Wipe Data
```
Check Cache, Dalvik, Data, Metadata, then Swipe
```

5. Flash the ROM
```
Choose /path/to/lineage-24.0-xxxxxxxx-UNOFFICIAL-klee.zip, then Swipe
```

6. Format Data
```
Choose Format data, then type yes
```
