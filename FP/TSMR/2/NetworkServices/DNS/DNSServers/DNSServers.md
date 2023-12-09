---
tags:
  - TSMR
  - TSMR_2
  - FP
  - DNS
  - IT
  - Networking
  - NetworkServices
  - ServerSoftware
  - LinuxSoftware
  - WindowsSoftware
  - Linux
  - Windows
---
# DNS Servers

For Unix-like OSes: [BIND](./BIND/BIND.md)
For Microsoft Windows: [BIND](./BIND/BIND.md), Windows Server DNS service

---
## DNS Types
### Primary (Master)
Primary DNS server are independent and manage their domain names directly.
They are directly managed using their configuration files where the server configuration files and domain name registers are stored.
Generally, primary DNS servers only manage few domain names each.
### Secondary
Secondary DNS servers replicate primary DNS servers.
These type of DNS servers exist to increase availability, one of the three pillars of cybersecurity.
In their configuration files it's defined what DNS servers to replicate.
### Cache / Hint
These servers store in cache storage the most recent and/or used Domain Name registries to provide faster times.
The difference between Cache and Secondary DNS servers is that secondary servers replicate fully one DNS server and like a primary one, a cache server only stores the needed registries in fast but volatile storage to make DNS queries more efficient over time.
### Forwarder

---
