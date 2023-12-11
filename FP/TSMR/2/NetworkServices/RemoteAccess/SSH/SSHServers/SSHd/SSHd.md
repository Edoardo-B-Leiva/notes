---
tags:
  - RemoteAccess
  - SSH
  - ServerSoftware
  - Linux
  - LinuxSoftware
  - FP
  - IT
  - Networking
  - NetworkServices
  - TSMR
  - TSMR_2
---
# SSHd
Stands for SSH daemon, it's the server for SSH connections.

default executable path: `/usr/sbin/sshd`
default configuration files: `/etc/ssh/`
	- `ssh_config.d/`
	- `sshd-config.d/`

- `Protocol <number>`
- `PermitRootLogin <yes/no>`
- `ListenAddress <IPv4 / IPv6>`
	`0.0.0.0` / `::` --> All hosts
- `HostKey <path/to/dir>`
- `KeyGenerationInterval <time>`
- `ServerKeyBits <number>`
	x < 512: **Not secure**
	x > 1024: Requires more computation power and time
- `AuthorizedKeyFile <path/to/dir>`
- `X11Forwarding <no/yes>`
- `Authentication`
- `Port <number>`
- `PasswordAuthentication <yes/no>`

Example configuration file for sshd:
```sshd_config
Protocol 2

Port 22
ListenAddress 0.0.0.0
ListenAddress ::

ServerKeyBits 2048
X11Forwarding no
PermitoRootLogin no
PasswordAuthentication no

HostKey /etc/ssh/ssh_host_dsa_key
HostKey /etc/ssh/ssh_host_rsa_key

StrictModes yes
Compression yes
```