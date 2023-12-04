---
tags:
  - IT
  - RemoteAccess
  - Networking
  - NetworkServices
  - TSMR
  - TSMR_2
---
# Telnet
Telnet (Telecommunication Network) permits the remote access to a CLI (Command Line Interface).
This protocol is no longer used nor pre-installed in common OSes since **its information is transmitted in plain text**, making it **unsecure** towards _network sniffing_ and _Man in the Middle_ attacks.
By default, the server _listens to network port `23`._

```sh
telnet <ip_address/domain_name> [<port>]
#--- Example command
telnet 127.0.0.1 23
```

```telnet
open <host> [-l user] [port]
close
quit
send <args>
set <target> <value>
```
