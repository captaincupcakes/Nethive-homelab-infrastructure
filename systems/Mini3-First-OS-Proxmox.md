# Mini PC 3

## Hardware Specs
- System: Lenovo Thinkcentre M75q Gen5
- CPU:AMD Ryzen 5 PRO 8500GE
- RAM:32GB DDR4
- Storage:512GB micron NVme
- GPU: AMD Phoenix2 [Integrated]

## Operating System
- Proxmox VE 9.2.2 x86_64
- Kernel version:Linux 7.0.2-6-pve

## Role in Lab
- Virtualization
- custom VM to run because we roll like that
- Custom Firewall (oncoming)
- VLAN
- Potential Seedbox

## Why Proxmox
- hearing so much of Virtualization. we delved into proxmox naturally, seeing my colleagues and senior administrators messing with
  VM's (and knowing one that has messed with proxmox), i delved in,this one is less linux messing (as i dealt with debian before)
  and more into the world of Virtual Machines, Virtual lan's and advanced networking in general.  im opening 2 branches at the same
  time here, and were going full steam

## Challenges
- Proxmox 9 uses .sources format instead of legacy .list files
  requiring different repo management commands than documented
  in most online guides

## Installed Software & Services
- nothing yet,just got it running


## Notable Configurations
- soon

## Lessons Learned
- Setting a custom network from an installer (never done that one before)
- Static IP configuration during OS installation
- Proxmox repository management (enterprise vs no-subscription)
- Disabling unused enterprise repos via .sources format
- Headless server management via web UI (port 8006)
- Proxmox subscription model and open source alternatives
