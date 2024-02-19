## Recovery Device Tree for the Samsung Galaxy S21 5G FE (Snapdragon)

## How-to compile it:

```sh
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_r9q-eng
make recoveryimage
```

Kernel source:
https://github.com/glikched/android_kernel_samsung_sm8350/tree/twrp-12.1

## TWRP functions list

Blocking checks:
- [x] Correct screen/recovery size
- [x] Working Touch, screen
- [x] Backup to internal
- [x] Restore from internal
- [x] reboot to system
- [x] ADB

Medium checks:
- [x] update.zip sideload
- [x] UI colors (red/blue inversions)
- [x] Screen goes off and on (T2W - Tap To Wake is broken)
- [x] F2FS/EXT4 Support, exFAT/NTFS where supported
- [ ] all important partitions listed in mount/backup lists
- [x] backup/restore to/from external (USB-OTG) storage (not supported by the device)
- [ ] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data (This might never be fixed)
- [ ] Correct date

Minor checks:
- [x] MTP export
- [x] reboot to bootloader
- [x] reboot to recovery
- [x] poweroff
- [x] battery level
- [x] temperature
- [ ] encrypted backups
- [x] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device)
- [x] USB mass storage export
- [x] set brightness
- [x] vibrate
- [x] screenshot
