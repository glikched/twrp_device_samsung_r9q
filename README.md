## Recovery Device Tree for the Samsung Galaxy S21 5G FE (Snapdragon)

## How-to compile it:

```sh
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_r9q-eng
make recoveryimage
```

Kernel source:
https://github.com/mohammad92/android_kernel_samsung_r9q
