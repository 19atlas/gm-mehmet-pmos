# device-gm-mehmet
PostmarketOS configuration files for General Mobile E-tab 4/willow
https://wiki.postmarketos.org/wiki/Porting_to_a_new_device

# files
- `build.prop` is came from rom
- `exynos4412-mehmet.dts` is for mainline kernel (WIP)
- `recovery.img` is twrp for etab4

## device info:
- General Mobile E-tab 4 (but it based on samsung)
- soc: exynos4412
- panel: LTN101AL03 `CONFIG_FB_S5P_LTN101AL03=y` ` CONFIG_BACKLIGHT_PWM=y`
- `CONFIG_TOUCHSCREEN_ATMEL_MXT1664S=y`
- `CONFIG_BT_BCM4334=y`
- `CONFIG_INPUT_YAS_ACCELEROMETER=y`
- `CONFIG_MFD_MAX77686=y (regulators confirmed)` also rtc
- Ram: 774 MB `40000000-7fefffff : System RAM`
- detected HSCDTD007/008 geomagnetic field sensor
- `s3cfb`
- `max77686`
- pcpu-alloc: s6720 r8192 d13760 u32768 alloc=8*4096
- root partition /dev/mmcblk0p10

## device partition:
```
Filesystem                Size      Used Available Use% Mounted on
tmpfs                   388.1M      8.0K    388.1M   0% /dev
tmpfs                   388.1M     16.0K    388.1M   0% /tmp
/dev/block/mmcblk0p8    438.0M      7.5M    430.5M   2% /cache
/dev/block/mmcblk0p10
                         13.2G    161.7M     13.1G   1% /data
/dev/block/mmcblk0p10
                         13.2G    161.7M     13.1G   1% /sdcard
/dev/block/mmcblk0p9    688.9M     11.7M    677.3M   2% /system
```

- more info [in postmarket wiki](https://wiki.postmarketos.org/index.php?title=User:Knuxify/Scratchpad&oldid=56232)
- more info cpu [here](http://web.archive.org/web/20200217083856/linux-exynos.org/wiki/Samsung_Exynos_4412)
