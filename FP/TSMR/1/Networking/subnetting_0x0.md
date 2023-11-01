[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io) (01/11/2023 Wed - x)
# Sub-netting: 0x0

## IP addresses

### IPv4
- Composed by ___32 bits___
- Divided in 4 octets \* 8 bits:
  - From 0 to 255 in decimal format each octet;
  - From 00 to FF in hexadecimal format each;
  - From 00000000 to 11111111 in binary format each;
- Total of possible IPv4 addresses: 4'294'967'296 (2^32)
### IPv6
- Composed by ___128 bits___
- Divided by 8 sextets with 16 bits:
     - From 0 to 65535 in decimal format each;
     - From 0000 to FFFF in hexadecimal format each;
- Total of possible IPv6 addresses: 3.40282366921e+38 (2^128)
---
## IP Classes

IPv4 addresses can be categorized in Classes.
Classes define what part of an IPv4 address indicates the connected host and what part of the address indicates the network in which the host is connected to.
There are a total of 5 possible classes, identifiable by a letter ranging from A to E.
>Classes can be identified by the "leading bits" when reading the IP in binary format.
### Class A
* Ranges from 0.0.0.0 to 127.255.255.255
* Leading bits: 0000...
* The first octet (the first 8 bits of the IP address) defines the network.
* `00000000|00000000.00000000.00000000`
### Class B
* Ranges from 128.0.0.0 to 191.255.255.255
* Leading bits: 1000...
* The first 2 octets (16 bits) define the network
* `10000000.00000000|00000000.00000000`
### Class C
* Ranges from 192.0.0.0 to 223.255.255.255
* Leading bits: 1100...
* 3 octets (24 bits) define the network and only 8 define the host.
* `11000000.00000000.00000000|00000000`
### Class D - Multicast ID
* Ranges from 224.0.0.0 to 239.255.255.255 
* Leading bits: 1110...
* These IP addresses have not a host identifier part.
* `11100000.00000000.00000000.00000000`
### Class E
* Ranges from 240.0.0.0 to 255.255.255.255
* Leading bits: 1111...
* Like class D IP addresses, these IPs do not have a host identifier part.
* `11110000.00000000.00000000.00000000`
* Reserved for experimental features and Research purposes.
---
## Subnet Masks
Subnet masks make the definition between host and network identifiers much more precise, which allows to create networks specifically made for ***anyone's*** needs.
This sub-netting is represented in 2 ways:
### Subnet mask
The subnet mask is represented like an IPv4 IP address, but it's better when seen in binary format:
- The 1s and 0s in this representation give information if the corresponding bit should be used as either a network or a host identifier.
- This format is useful enough but it's limited to IPv4 and it's time consuming to represent.
###### Example for a subnet mask:
`10.123.135.12, 255.0.0.0`

### CIDR notation
The CIDR notation uses the same principle of the subnet mask but it's represented in a more concise and less limited way making it easier to use and can be used with IPv4 as well.
###### Example:
`10.123.135.12/8`  
The number after the IP address is the CIDR notation, it indicates how many bits are used for subnet identification, counting from left to right.

---
## NAT & PAT
NAT and PAT are the base for local networks (LANs) as how we now know it.  
NAT permits the assignation of IP within preset ranges (a.k.a. Private IP addresses) in a local network in order to preserve IP addresses.  
PAT permits the tunneling of ports between the Public IP for the network and the Local IP of a specific machine.  

NAT alone limits the possibility to serve because of this discrepancy in understanding who is what, PAT helps this by assigning specific ports as open for the public IP
a port for a specific private IP.

In the example below we can see this association.  
When an outside client tries to make a request for the server inside the private network, the PAT comes in place to "tunnel" the data from the router's port 8080 to the actual server's port 8080.
###### Example:
`10.0.0.10/8:8080 -> 17.29.4.106:8080`
This also works with ports that are not the same in both ends, in that case the client will need to make the request to the port corresponding to the router one.
---
