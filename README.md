# TWRP Device configuration for Motorola Moto G9 Power

## Device specification

Basic   | Spec Sheet
-------:|:------------------------
CPU     | Octa-core (4x2.0 GHz Kryo 260 Gold & 4x1.8 GHz Kryo 260 Silver)
CHIPSET | Qualcomm SDM662 (SM6115 "Bengal") Snapdragon 662
GPU     | Adreno 610
Memory  | 4GB
Shipped Android Version | 10.0
Storage | 64GB
Battery | 6000 mAh
Dimensions | 172.1 x 76.8 x 9.7 mm
Display | 720 x 1640 pixels, 20.5:9 ratio
Rear Camera  | 64 MP, f/1.8, 26mm (wide), 1/1.97", 0.7µm, PDAF + 2 MP, f/2.4, (macro), AF + 2 MP, f/2.4, (depth)
Front Camera | 16 MP, 1.0µm

![Device Picture](https://fdn2.gsmarena.com/vv/bigpic/motorola-moto-g9-power.jpg)


### Kernel Source
Check here:

https://github.com/mistersmee/android_kernel_motorola_cebu/


### How to compile

```sh
. build/envsetup.sh
export LC_ALL=C
lunch omni_cebu-eng
mka -jX clobber && mka -jX recoveryimage
```
Note: 'X' in `mka -jX recoveryimage` is the number of cores your processor has.
For example, a quad-core processor would have `mka -j4 recoveryimage` as the command.

### Copyright
 ```
  /*
  *  Copyright (C) 2013-21 The OmniROM Project
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  *
  */
  ```
