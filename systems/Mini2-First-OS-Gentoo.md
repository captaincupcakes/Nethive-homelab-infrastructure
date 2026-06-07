# MiniPC 2 

## Hardware Specs
- PC:Dell Wyse 7040
- CPU:Intel(R) Core(TM) I5-6500TE (4) @ 3.30GHz
- RAM:8GB RAM
- GPU:Intel HD Graphics 530 @ 1.00 GHz [integrated]
- Storage: 2 TB 2.5 SSD

## Operating System
- Old Systems tried:Void Linux
- Current: Gentoo Linux x86_64
- Kernel Version:Linux 6.18.18-gentoo-dist
- Desktop Environment:KDE Plasma 6.5.5

## Role in the lab
- Test system
- See how distros perform and behave
- QC and system damage/recovery simulation

## Why Gentoo
- If the self of the past thought that arch was hard and confusing at the beginning, then he certainly would of raged with gentoo,
  After trying arch and testing Void Linux, i wanted to push the envelope to the max, Enter Gentoo, with the experience i acquired
  in Eos, Gentoo Became a great teacher, it show me how an actual OS behaves underneath and made me understand syscalls, Flags and
  Optimal setups, every day i learn how wide the linux ecosystem is,yet Gentoo is "the framework to understand it all",it is after
  all, the professor for not only for learning and training for my career, but also the buddy who does this for the love of the game

## Installation Process
- first i struggled using cfdisk,but got a hang of it rather quick,the gentoo reminded me in a very stern voice why syntax matters,
  after that, use flags put me back to square one "used too many for not yet installed packages", nothing clicked until i backtracked,
  started adding flags as we went through. then the versions of gentoo got me,as i was adding stuff not available on the version i
  selected,fixed that and the final contender. GRUB.
- you see, GRUB is very versatile,but that was not the issue, the issue was that dell's, like 60-70% of the time do not obey the
  location of your EFI boot file,and default back to their desired location,that was a head breaker, struggled for hours,scouring
  forums, gave up and went next day to start from scratch, NO DICE, gave up and after extensive forum research, cross-referencing
  multiple sources to identify the root cause, turns out,most of dells have a bug where they default to their desired location no
  matter if you relocate the file right from the UEFI, they just straight up ignore your request and default. however,the versatility
  of GRUB meant i could send the boot file back to where the UEFI wanted it,without too much hassle, by running the following command:
  ```bash
  Grub-install --efi-directory=/efi --removable
  ```
  that fixed my issue and i was able to boot.
- however,as this machine is a test rig,it will get a new system soon,but i do enjoy gentoo, will definitely install in a laptop
  i plan to buy in the future for daily driving,id just have to set it very stable.
- also this test mini DOES NOT LIKE GENTOO, compilation times take forever, and the system slows down even for midsize apps/packages
  and i understand it,this machine was not made for this kind of stuff, it was made for office/POS/Data Handling/Light Work

## USE Flags

- COMMON_FLAGS="-O2 -pipe"
- CFLAGS="${COMMON_FLAGS}"
- CXXFLAGS="${COMMON_FLAGS}"
- FCFLAGS="${COMMON_FLAGS}"
- FFLAGS="${COMMON_FLAGS}"
- MAKEOPTS="-j6 -l4"
- USE="dracut postproc policykit gstreamer vaapi wayland dev-qt geoclue udev elogind X dbus qt pipewire kde-pla>

- Overrides the profile's ACCEPT_LICENSE default value
- ACCEPT_LICENSE="-* @FREE @EULA @GPL-COMPATIBLE @BINARY-REDISTRIBUTABLE"


- NOTE: This stage was built with the bindist USE flag enabled

- This sets the language of build output to English.
- Please keep this setting intact when reporting bugs.
- LC_MESSAGES=C.UTF-8
- GRUB_PLATFORMS="efi-64"
- VIDEO_CARDS=intel

## Challenges
- detailed above, compilation times are atrocious,not enough performance for this mini to handle that.also the UEFI
  Ignoring my requests, this machine is made for something light like Void Linux

## Current State
- Active

## Lessons Learned
- USE Flags
- Options of compiling vs binaries
- allocation of resources
- Proper Use of GRUB
- how a system is setup and what every step does
- Dell UEFI quirks and EFI boot path behavior
- Hardware limitation assessment and Workload matching

