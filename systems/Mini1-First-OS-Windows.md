# Windows Mini — Dell Wyse 7040
## Hardware Specs
- PC: Dell Wyse 7040
- CPU: Intel Core i5-6500TE (4) @ 3.30GHz
- RAM: 16GB DDR4
- GPU: Intel HD Graphics 530 [Integrated]
- Storage: 1.75TB HDD
- Display: Dell P2414H 1920x1080 24" 60Hz [External]

## Operating System
- OS: Windows 10 Enterprise LTSC 1809 x86_64
- Kernel: WIN32_NT 10.0.17763.7919
- Shell: PowerShell 5.1

## Role in Lab
- Windows testing and debugging environment
- Cross-platform compatibility testing
- Application behavior comparison vs Linux
- Network diagnostics from a Windows perspective

## Why Windows LTSC
- LTSC chosen for stability and minimal bloat
- No forced updates, no Store apps, no telemetry noise
- Clean environment for controlled testing scenarios

## Notable Configurations
- Ethernet only -  no WiFi
- Planned: M.2 WiFi card addition for bluetooth capability
- Static LAN configuration

## Challenges
- LTSC intentionally stripped of modern Microsoft tooling
- winget installation requires manual dependency resolution
  due to missing Store infrastructure

## Current State
- Active
- Uptime: 62 days
- Note:System reports extended uptime due to Windows counting sleep/hibernate cycles

## Lessons Learned
- Windows LTSC environment management
- PowerShell for system administration
- Dependency resolution on stripped Windows environments
- Cross-platform network troubleshooting
