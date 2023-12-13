---
tags:
  - SSH
  - RemoteAccess
  - ServerSoftware
  - IT
  - FP
  - Networking
  - NetworkServices
  - TSMR
  - TSMR_2
---
# SSH Tunnels
It's possible to pass your internet traffic though an SSH Tunnel to possibly make it more secure.
`ssh -L 10443:smtp.gmail.com:443 user@hostname.domain`
It uses SSH to stream data to the client creating a secure section of the connection to the final peer / server.