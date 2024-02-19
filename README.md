# device-gm-mehmet
PostmarketOS configuration files for General Mobile E-tab 4/willow
https://wiki.postmarketos.org/wiki/Porting_to_a_new_device

## device info:
- General Mobile E-tab 4 (but it based on samsung)
- soc: exynos4412
- panel: LTN101AL03 `CONFIG_FB_S5P_LTN101AL03=y` ` CONFIG_BACKLIGHT_PWM=y`
- `CONFIG_TOUCHSCREEN_ATMEL_MXT1664S=y`
- `CONFIG_BT_BCM4334=y`
- `CONFIG_INPUT_YAS_ACCELEROMETER=y`
- `CONFIG_MFD_MAX77686=y (regulators confirmed)` also rtc
- it's also mfd
- more info [here](http://web.archive.org/web/20200217083856/linux-exynos.org/wiki/Samsung_Exynos_4412)
