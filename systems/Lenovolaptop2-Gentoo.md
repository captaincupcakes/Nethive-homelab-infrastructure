# Lenovo Laptop 2 - Gentoo

## Hardware Specs
- System: Lenovo Thinkpad L15 gen 2a 20X70056US
- CPU:AMD Ryzen 7 PRO 5850U (16) @ 4.51 GHz
- RAM:32GB DDR4-3200
- Storage:1TB SSD
- GPU:AMD Radeon Vega Series / Radeon Vega Mobile Series [Integrated]

## Operating System
- Gentoo Linux x86_64
- Kernel version:Linux 6.18.43-gentoo-dist-bin (i value my time too much to compile kernels)
- Desktop Environment:KDE Plasma 6.6.6

## Role in Lab
- Messing even more with gentoo
- 3rd in command if any other go down
- curating/customizing O/S even more
- whole suite of apps as well for a backup system

## Why Gentoo Again
- this one is less gentoo and more lenovo..somehow lenovos have this reputation right next to framework laptos
  the ultimate lego so to say. so i got an offer on 2 for a very nice price,and i jumped right in, so far,the
  customizations hardware wise is something ive never seen before,im used to customizing cars,not laptops.but
  im in.

## Installed Software & Services
- Alacritty
- Firefox
- Thunar
- Vlc
- Emacs
- Qalculate

## Notable Configurations
- to be added

## Lessons Learned
- Great WiFi signal, what happens when a company puts effort in building a laptop
- Realtek does not play nice with linux,didnt have issues but changed to intel for Wifi due to concerns
- unlike the dell.lenovo respect the OS's efi location

## Use Flags

- COMMON_FLAGS="-O2 -pipe"
- CFLAGS="${COMMON_FLAGS}"
- CXXFLAGS="${COMMON_FLAGS}"
- FCFLAGS="${COMMON_FLAGS}"
- FFLAGS="${COMMON_FLAGS}"
- MAKEOPTS="-j17 -l16"

- USE="dracut postproc policykit gstreamer vaapi wayland dev-qt geoclue udev elogind X dbus qt pipewire kde-plasma bluetooth networkmanager acpi"

- ACCEPT_LICENSE="-* @FREE @EULA @GPL-COMPATIBLE @BINARY-REDISTRIBUTABLE"

- LC_MESSAGES=C.UTF-8

- GRUB_PLATFORMS="efi-64"

- VIDEO_CARDS="amdgpu radeonsi"

## Current state
- Active

