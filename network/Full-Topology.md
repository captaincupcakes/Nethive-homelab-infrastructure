# Network Topology
## Hardware
- Router: Netgear Nighthawk RAX50
- Switch 1 (Upstairs): TP-Link TL-SG108 (unmanaged)
- Switch 2 (Downstairs): TP-Link TL-SG108 (unmanaged)

## Layout
```
ISP
└── Netgear Nighthawk RAX50
├── Switch 1 (Upstairs)
│     ├── Xerox WorkCentre 6605DN (Network Printer)
│     └── Zebra GK420D (Label Printer)
├── Switch 2 (Downstairs)
│     ├── Nobara Rig (Main Workstation)
│     ├── Gentoo Mini — MiniPC 1 (Test/Lab)
│     └── Windows Mini — MiniPC 2 (Testing/Debug)
└── WiFi
└── EndeavourOS Laptop (poor signal —
antenna placement issue, extended
router antenna to main hall as
temporary mitigation)
```

## Current Limitations
- Both switches are unmanaged — no VLAN support yet
- WiFi signal weak at laptop due to MSI antenna placement
- No network segmentation currently

## Planned Improvements
- TP-Link TL-SG108E managed switch → enable 802.1Q VLANs
- Planned VLAN segmentation:
  - VLAN 10 → Main devices
  - VLAN 20 → Lab/experimental machines
  - VLAN 30 → IoT/printers
- pfSense/OPNsense on dedicated mini PC for inter-VLAN routing
- M.2 WiFi card on Windows Mini for Bluetooth

## Lessons Learned
- Physical network planning across multiple floors
- Printer network integration (wired preferred for reliability)
- WiFi signal diagnosis and mitigation
- Planning for future network segmentation
