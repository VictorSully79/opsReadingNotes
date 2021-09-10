# VirtualBox Network Settings: Complete Guide

notes taken from above named article:<https://www.nakivo.com/blog/virtualbox-network-setting-guide/>

VirtualBox provides several different network settings:

- Not Attached
- NAT
- NAT Network
- Bridged Adapter
- Internal Network
- Host-Only Adapter
- Generic Driver

Each VM can have up to 8 virtual adapters.

There a 6 virtual adapter types:

- AMD PCnet-PCI II (Am79C970A). This network adapter is based on AMD chip and can be used in many situations. As for Windows guests, this network adapter can be used for older Windows versions (such as Windows 2000) because newer Windows versions such as Windows 7, 8 and 10 do not contain a built-in driver for this adapter. Originally, the
- Am79C970A PCI device contained a single chip 10-Mbit controller and the DMA engine was integrated. This network adapter also supports AMD’s Magic Packet technology for remote wake-up.
- AMD PCnet-FAST III (Am79C973). This virtualized network adapter is supported by almost all guest operating systems that can run on VirtualBox. GRUB (the boot loader) can use this adapter for network boot. Similarly to the previous network adapter, this one is based AMD chip.
- Intel PRO/1000 MT Desktop (82540EM). This adapter works perfectly with Windows Vista and newer Windows versions. The most of Linux distributions support this adapter as well.
- Intel PRO/1000 T Server (82543GC). Windows XP recognizes this adapter without installing additional drivers.
- Intel PRO/1000 MT Server (82545EM). This adapter model is useful to import OVF templates from other platforms and can facilitate import process.
Paravirtualized Network Adapter (virtio-net) is a special case. Instead of virtualizing networking hardware that is supported by most operating systems, a guest operating system must provide a special software interface for virtualized environments. This approach allows you to avoid the complexity of networking hardware emulating and, as a result, can improve network performance.

## VirtualBox Network Modes

- Not attached
  
- NAT
  
- NAT Network

- Bridged Adapter

- Internal Network

- Host Only Adapter

- Generic Driver