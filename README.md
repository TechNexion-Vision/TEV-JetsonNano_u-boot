## TEV JetsonNano u-boot tweak
### Folder location(created by TEV-Jetson_Jetpack_script)
```
<nvidia_folder>/Linux_for_Tegra/sources/u-boot
```

&nbsp;

### Compile script
It will create **u-boot.bin**.
``` coffeescript
$ ./compile_u-boot.sh
```

### Take effect
1. Copy u-boot.bin
Copy **u-boot.bin** to:
```
<nvidia_folder>/Linux_for_Tegra/bootloader/t210ref/p3450-0000/u-boot.bin
```
2. Remake system.img and flash into device.
* For Xavier-NX
```coffeescript
$ sudo ./flash.sh jetson-xavier-nx-devkit-emmc mmcblk0p1 
```
* For Nano
```coffeescript
$ sudo ./flash.sh jetson-nano-devkit-emmc mmcblk0p1 
```
