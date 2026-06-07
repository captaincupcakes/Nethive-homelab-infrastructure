# Nobara Rig

## Hardware Specs
- Motherboard: Asus TUF Z390(WiFi)
- CPU:Intel(R) Core(R) I9-9900K (16) @ 5.00 GHz
- RAM:Corsair Dominator Platinum 64GB DDR4
- GPU:AMD Radeon RX 7900 XTX (previously rocked a Nvidia RTX 2080Ti Founders edition)
- Storage:x1 NVMe 4TB Drive, x1 2.5GB Samsung SSD
- Cooling:Corsair H150i
- Drives/media:x1 HL-DT-ST BD-RE BH16NS40 BD Drive, x1 HL-DT-ST BD-RE WH14NS40 BD Drive
  Multi Card Reader.
- Case:Phanteks Enthoo 2 case
- PSU:Corsair RMx RM1000x 1000w 80 PLUS GOLD power supply

## Operating System
- Old systems tried and tested: Linux Mint 20 Cinnamon, Fedora 38 KDE
- Current:Nobara Linux 43 (KDE Plasma Desktop edition) x86_64
- Kernel version:Linux 7.0.1-200.nobara.fc43.x86_64
- Desktop Environment:KDE Plasma 6.6.4

## Role in Lab
- Main Support.
- works as the data backup.
- Compiler/heavy tasks manager (it can handle it)
- Gaming system (plays them really well)
- recovery machine (for when one of the other systems goes down).

## Why Nobara
- I chose nobara for multiple reasons, fedora was my first branch out of the debian ecosystem,
  and it had the blend i was looking for, cutting edge (not "stable" but not bleeding edge),
  was easy to use and it rarely goes down,if at all, however the community made some decisions i
  did not approve of,but it was just that nice to let go. Enter Nobara, all the goodness of fedora,
  but an even wider team that supports you,cares about you,even better, fine tuned the system for
  the best gaming experience.


## Setup Process
- liquidctl - AIO cooling management via CLI
- ckb-next - Corsair Peripheral Management on Linux
- Vivaldi/Firefox/Librewolf - Layered browser setup
- Steam + Wine - Gaming and Windows compatibility
- blender - 3D rendering for potential 3D printer addition
- Filezilla and Dolphin - Configured for seedbox management

## Notable Configurations
- AIO setup and  systemd service for liquidctl
- Intel ME disable
- CUPS - configured for network printing across lab machines

## Intel ME Disable
- Disabled Intel Management Engine by Blacklisted mei, mei_me kernel modules via /etc/modprobe.d/
- reducing attack surface on the primary workstation.
- Rebuilt initramfs using dracut --force post-configuration.

## Challenges
- this device is the one that has given me the least trouble.every once in a blue moon
  it borks due to an update,but going into live and restoring the system is not much trouble

## Lessons Learned
- AMD vs Nvidia driver management on Linux
- systemd service creation and management
- Hardware-level security configuration (Intel ME)
- System recovery via live environment
- Cross-platform application compatibility via Wine

## Current State
- Active
