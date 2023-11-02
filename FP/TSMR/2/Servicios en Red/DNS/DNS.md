[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io) (02/11/2023 Thu - x)
# DNS
**DNS** (_Domain Name Service_) is, as the name implies, a service which main purpose is to **provide an IP address corresponding to the given Domain Name**.
This is also, in today's day and age, one of the basic information given from a [DHCP server](../DHCP/DHCP.md).
## Brief introduction to Domain names
Example:
`www.google.com -> 142.250.200.100`
Domain names help us by not needing to remember IP addresses.
It's much easier to remember "www.google.com" instead of "142.250.200.100".
## Domain Name Levels
Domain Names are structured in "levels"
### Domain Root
Starting with the root level which is " ", in fact, DNs should finish in `example.com. ` instead of `example.com`.
### TLDs
Right after that there's the TLDs (Top Level Domains) which are generally 2, 3 or 5 characters long.

**_Examples_**: `.com, .es, .net, .org, .cc, .io, .uk, etc.`

TLDs cannot be owned by End-Users, only authorized entities.

**_Example:_**
```
.com: cannot be owned by me.
example.com: could be owned by me.
```
TLDs can be categorized by their meaning:
- **gTLD**: General purpose (anyone can own them): `.com, .net`
- **ccTLD**: Country Code TLDs: `.it, .es, .jp, .us, .uk, .ca, etc.`
### IDN
Some institutions and governments serve Domains ending with a second level domain name, giving third level domains

**_Examples:_**
`.co.uk, .co.jp, .com.co, etc.`
## Tools
To manually look for an IP address starting from its Domain Name, there are multiple tools available both offline and online.
## FQDN
FQDN (a.k.a. Fully Qualified Domain Name) is the combination of a machine's Domain Name and its hostname.

**_Example_**: 
```
Hostname: iac.cc;
Domain Name: upv.es;
FQDN: iac.cc.upv.es;
```
## Register types
A DNS Server provides a different response depending on the type of register it has saved.
The most commonly known are:
- **A**: IPv4 Association `IPv4 Address -> Domain Name`
- **AAAA**: IPv6 Association `IPv6 Address -> Domain Name`
- **CNAME**: Canonical Name `Domain Name -> Domain Name`
- **PTR**: Points an IP address to Domain name instead of a Domain name to an IP address. `Domain Name -> IP address`
- **SRV**: Specific service, requires extra parameters such as:
  - Port
  - Priority
  - etc.
- **MX**: Mail Exchange, used to point to an SMTP Server.

# DNS Servers
## BIND 9
### Introduction
BIND 9 is a DNS Server software made by the BSD (Berkeley University Software Distribution).
Installable in both Linux, BSDs and Windows Server.

Its configuration files are located in: `/etc/bind/named.conf`  
On MS Windows it's located in: `C:\Windows\system32\dns\etc\named.conf`

### Global configuration file
- `allow-query { xxx.xxx.xxx.xx ; any; none; } ;` 
- `allow-transfer { xxx.xxx.xxx.xxx; none; any ; } ;`
- `zone "zone_name" { options...; } ;`
  - `type <type>;`
  - `file </path/to/db.domain.com>;`