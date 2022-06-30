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
1. Copy **u-boot.bin** to:
```
<nvidia_folder>/Linux_for_Tegra/bootloader/t210ref/p3450-0000/u-boot.bin
```
2. flash new u-boot partition into device.
```coffeescript
$ sudo ./flash.sh -r -k LNX jetson-nano-devkit-emmc mmcblk0p1
```
