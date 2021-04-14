# Genchu_kernel
Genchu kernel boot logo patchset


![Genchu kernel boot logo](https://dev.gentoo.org/~alicef/genchu_boot_logo.png)


### Quick start
```
genchu linux # genkernel --kernel-ld=ld.bfd --kernel-config=.config_genchu --luks --lvm --splash --menuconfig all
genchu linux # qemu-system-x86_64 -smp 4 -kernel /boot/kernel-genkernel-x86_64-5.4.110-gentoo -initrd /boot/initramfs-genkernel-x86_64-5.4.110-gentoo -m 1G -append "vga=extended" -vga cirrus -display gtk,gl=on -machine accel=kvm
```
