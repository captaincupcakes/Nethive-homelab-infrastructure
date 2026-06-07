# EOS Laptop

## Hardware Specs
- System: MSI Creator 15 A10SFS REV:1.0
- CPU:Intel i7-10875H (16) @ 5.100GHz
- RAM:32GB DDR4 (was planning on upgrading to 64GB,Alas)
- Storage:1TB SSD (alas,ran out of time)
- GPU:Intel CometLake-H GT2 [UHD Graphics]
- GPU:NVIDIA GeForce RTX 2070 SUPER Mobile / Max-Q

## Operating System
- EndeavourOS Linux x86_64
- Kernel version:7.0.5-arch1-1
- Desktop Environment:Plasma 6.6.4

## Role in Lab
- For when i need a proper computer elsewhere,or im lazy and dont want to use my rig
- Performs well for emulators or light gaming
- First backup when the rig goes down
- Network testing and sharing
- Git/documentation (for the time being, will add my rig to the list)

## Why EndeavourOS
- ever since i got involved with Linux, ive heard/seen the "impossibility" of Arch and how
  High-tech you had to be to install it, once i decided to branch out of debian-based distros
  arch was my first go to,armed with nothing more than a live DVD, off i went,but it ended in failure,
  was still too immature to handle CLI, but as stubborn and curious as i am, never gave up and instead
  i branched out to find arch based distros. Enter EndeavourOS, basically arch with an installer. Off
  i went and while i thought "this is it,ive installed arch" and was ready to move to the next OS,i
  decided to stick around, and what an experience it was, Eos and Arch show me what it actually meant to
  "use the terminal", over time,everything clicked,and started to get more in depth (i even managed to break it
  on purpose), and it broke on updates too, but that experience taught me a lot of knowledge on how to recover from
  a bad update,or a borked kernel, once i had "the juice", linux started clicking even more, not only did i wanted
  to go for full obscure distros, bleeding edge made everything look outdated by comparison, surprisingly, it hasnt given
  me much trouble for a long time.

## Installed Software & Services
- Samba client
- Git
- Wine
- Steam

## Notable Configurations
- envycontrol -  GPU switching between Intel and NVIDIA modes
- Dual GPU management (Intel UHD + RTX 2070 Max-Q)
- Samba client configured for lab file sharing

## Lessons Learned
- Arch-based system recovery from bad updates and borked kernels
- Dual GPU management on Linux laptops
- Network signal diagnosis and hardware investigation
- Rolling release maintenance discipline

## The Bad WiFi Issue
- Wireless only-poor signal due to old house made of thick wood
- Wired ethernet available, only used for hard testing or troubleshooting
- Router Antenna extended to Main hall to improve signal
- Most devices do get good signal,except the laptop, measured with wifi signal strength app
  suspect my laptop antennas or the card are giving issues..
- update: antennas are in a very bad location on the laptop (end of the case, both right near each other)
  engineering a way to add external stubby antennas, guess MSI went the cheap route when it came to WiFI
