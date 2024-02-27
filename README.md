# device-gm-mehmet
PostmarketOS configuration files for General Mobile E-tab 4/willow
https://wiki.postmarketos.org/wiki/Porting_to_a_new_device <br>
twrp ile flashlanma tavsiye edilir

## FOR MAINLINE SUPPORT
mainline a yönelik dal
## envkernel.sh yöntemiyle
- `make -j$(nproc)` # kernel derle
- `pmbootstrap build --envkernel linux-postmarketos-exynos4` # pmos derle
- `pmbootstrap install --android-recovery-zip --recovery-install-partition=data` # bu twrp flashlama için
