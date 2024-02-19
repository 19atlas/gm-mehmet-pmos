# device-gm-mehmet
PostmarketOS configuration files for General Mobile E-tab 4/willow
https://wiki.postmarketos.org/wiki/Porting_to_a_new_device

## device info:
- General Mobile E-tab 4 (but it based on samsung)
- soc: exynos4412
- panel: LTN101AL03
- `CONFIG_TOUCHSCREEN_ATMEL_MXT1664S=y`
- `CONFIG_BT_BCM4334=y`
- more info [here](http://web.archive.org/web/20200217083856/linux-exynos.org/wiki/Samsung_Exynos_4412)

## ERROR
```
Assembler messages:
/home/pmos/build/src/Whispermehmet_VE-82c800ec59a0a4acbbbf473591ea4e70eef80c05/arch/arm/mm/proc-v7.S:522: Error: junk at end of line, first unrecognized character is '#'
```
