
# Asus-ROG-STRIX-Z270H-DSDT-Patch

 Hackintosh on Asus ROG Strix Z270H
 Current OS: macOS Catalina 10.5.5

## Hardware

 CPU: Intel i5 7600K

 GPU: Intel HD630 (iGPU, enabled), Nvidia GTX 1060 3GB (eGPU, disabled)

 RAM: 2X8GB GSKILL DDR4 2400CL15

 Motherboard: ASUS ROG STRIX Z270H

 Audio Codec: SupremeFX S1220A

 Ethernet Card: Intel I219V

 Wifi/BT Card: DW1560

 What guide/tool followed: [opencore 0.5.9](https://dortania.github.io/OpenCore-Install-Guide) or [clover 5120](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/)

 What part I got an issue with:

 1. Intel HD630: Pink Screen issue. Followed the guide [here](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/config.plist-per-hardware/coffee-lake#pink-purple-tint).
 
 2. Disabled Nvidia GTX 1060. Followed the guide [here](https://dortania.github.io/OpenCore-Install-Guide/extras/spoof.html#deviceproperties-method) for opencore, clover was also similar.
 
 3. Motherboard was not booting and getting stuck at #LOG:EXITBS:START but fixed with the options seen on this [commit](https://github.com/brosahay/Asus-ROG-STRIX-Z270H-DSDT-Patch/commit/c82882697983e746bfa0c8ee6cc9bde210e2b9d1). The option "SyncRuntimePermissions" also helped fixing dual boot issues with Windows 10.
