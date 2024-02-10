# TWRP Device Tree for Samsung Galaxy S21 FE 5G

The Galaxy S21 FE 5G (codenamed _"r9q"_) is an upper-mid-range smartphone from Samsung.

It was announced and released in January 2022.

There are also a few more different variant, but all of them are classified as r9q and share almost the same hardware.

## Device specifications

| Feature                        | Specification                                                                             |
| -----------------------------: | :---------------------------------------------------------------------------------------- |
| Chipset                        | Qualcomm SM8350 Snapdragon 888                                                            |
| CPU                            | Octa-core (1x2.84 GHz Cortex-X1 & 3x2.42 GHz Cortex-A78 & 4x1.80 GHz Cortex-A55)          |
| GPU                            | Qualcomm Adreno 660                                                                       |
| Memory                         | 6GB / 8GB RAM (LPDDR4X)                                                                   |
| Shipped OS                     | Android 12 (One UI 4.1)                                                                   |
| Storage                        | 128GB / 256GB (UFS 2.1)                                                                   |
| SIM                            | Single SIM (Nano-SIM) or Dual SIM (Nano-SIM, dual stand-by)                               |
| Battery                        | 4500mAh Li-Ion (non-removable), 25W fast charge                                           |
| Dimensions                     | 155.7 x 74.5 x 7.9 mm (6.13 x 2.93 x 0.31 in)                                             |
| Display                        | 6.4”, 1080 x 2340 pixels, 19.5:9 ratio, Super AMOLED, 120Hz (~403 ppi density)            |
| Rear Camera 1 (IMX555/S5K2LD)  | 12 MP, f/1.8, 26mm (wide), 1/1.76", 1.8µm, Dual Pixel PDAF, OIS                           |
| Rear Camera 2 (IMX258/HI1336C) | 12 MP, f/2.2, 13mm, 123˚ (ultrawide), 1/3.0", 1.12µm                                      |
| Rear Camera 3 (HI847)          | 8 MP, f/2.4, 76mm (telephoto), 1/4.5", 1.0µm, PDAF, OIS, 3x optical zoom                  |
| Front Camera (IMX616)          | 32 MP, f/2.2, 26mm (wide), 1/2.74", 0.8µm                                                 |
| Fingerprint                    | Goodix GW9558 (under display, optical)                                                    |
| Sensors                        | Accelerometer, Gyro, Proximity (virtual), Compass, Hall IC, Grip                          |
| Extras                         | Dual speakers, NFC                                                                        |

## Device picture

*TODO: Add a picture of Samsung Galaxy S21 FE (r9q)

## Kernel source 

Available at [https://github.com/glikched/android_kernel_samsung_sm8350/tree/twrp-12.1](glikched/android_kernel_samsung_sm8350)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/glikched/android_device_samsung_r9q.git -b android-12.1 device/samsung/r9q
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_r9q-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2024 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```
