# jetson os

- https://www.forecr.io/blogs/installation/jetpack-5-1-installation-for-dsboard-ornx


## prereq

virtual machine with ubuntu 20.04 server

```
sudo snap install task --classic

```


## build environment

- create .env from env.sample

- download jetson, bsp, rootfs and build rootfs
```
task build
```

bsp for dsboard-ornx in runtime/Linux_for_Tegra
```
./kernel/Image
./kernel/dtb/tegra234-p3767-0000-p3768-0000-a0-hdr40.dtbo
./kernel/dtb/tegra234-p3767-0000-p3768-0000-a0.dtb
./kernel/bootloader/tegra234-mb1-bct-gpio-p3767-dp-a03.dtsi
./bootloader/t186ref/tegra234-bpmp-3767-0000-a02-3768-0000-a00.dtb
./bootloader/t186ref/BCT/tegra234-mb1-bct-pinmux-p3767-dp-a03.dtsi
./bootloader/t186ref/BCT/tegra234-mb1-bct-padvoltage-p3767-dp-a03.dtsi
./jetson-orin-nx-devkit-16gb.conf
./p3768-0000+p3767-0000.conf
```

## customize rootfs

add user ubuntu, etc.
```
task customize
```
