# kernel-fragments

```sh
cd /usr/src/linux
make clean 
make mrproper
make x86_64_defconfig
./scripts/kconfig/merge_config.sh -n .config ~/sources/kernel-fragments/*.config
genkernel all
grub-mkconfig -o /boot/grub/grub.cfg
```
