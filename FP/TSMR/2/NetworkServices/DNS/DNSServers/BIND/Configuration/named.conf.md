---
tags:
  - DNS
  - FP
  - IT
  - Linux
  - LinuxSoftware
  - Networking
  - NetworkServices
  - ServerSoftware
  - TSMR
  - TSMR_2
---
# named.conf
`named.conf` is the main configuration file for BIND.
The default path for this configuration file are:
- Linux: `/etc/bind9/named.conf`
- MS Windows: `C:\windows\system32\dns\etc\named.conf` (By default this config file **DOES NOT EXIST** and must be created)
- Mac OS: `/var/named/named.conf`
>In this file \*, \? and \! are supported.

The general content format is:
`<setting_name> <value> ;`
`<setting_name> { <values and settings> ; ... ; } ;`
Semicolons (`;`) are used to mark the end of a configuration statement and are required.


- `allow-query {<IPs>}`: defines what hosts are allowed to send queries to the server, this includes cache DNS servers.
- `allow-transfers {<IPs>}`: defines what secondary servers are allowed to make transfers to the server.
- `recursion <yes / no>`: if enabled, it allows recursive DNS queries, or else only iterative will be allowed.
- `directory "<path/to/file>"`: defines the path to additional config files.
- `blackhole {<IPs>}`: 
- `zone "<name>" {...}`: Defines a zone and its
- `type <type>`: Defines the type the server is and its behavior.
- `file "<path/to/file>"`: defines the path to a zone configuration file

Example configuration file:
```named.conf
allow-query {*;};
allow-transfer {!*;};
recursion yes;
blackhole {127.*.*.*;};
zone 
```