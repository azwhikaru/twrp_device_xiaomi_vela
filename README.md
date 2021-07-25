XiaoMi CC9 Meitu Edition
===============
```
By : Hikaru & liangsheng8708
```
The XiaoMi CC9 Meitu Edition (codename _"vela"_) is a Smartphone from XiaoMi.

This is a Minimal Device Tree for building TWRP for XiaoMi XiaoMi CC9 Meitu Edition (Codename: vela). I used TWRP by multirom and TWRP for XiaoMi 9 Lite from rakomancha to finally build a working tree for XiaoMi CC9 Meitu Edition.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A75 | Eight-Core | SDM710
Memory       | 8GB RAM
Shipped Android Version | 10.0 (Q)
Storage      | 256GB UFS2.1
Display      | 6.39

This branch is for building TWRP.

### Thanks to:
 * liangsheng8708
 * Myself

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create xiaomi/vela. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch vela-eng

make clean && make recoveryimage
```
