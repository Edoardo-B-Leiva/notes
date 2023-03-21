# Subnetting: 0x0

## IP addresses

* IPv4

	* 32 bits
	* 4 octets \* 8 bits (from 0 to 255)
	* Total of possible IPv4 addresses: 4.294.967.296 (2^32)

* IPv6

	* Composed by 128 bits
	* Divided by 8 hextets with 16 bits each (from 0 65535)
	* Total of possible IPv6 addresses: 3.40282366921e+38 (2^128)

---
## IP Classes

>IPv4 Classes are a deprecated concept and are used as a generalization for Subnet masks

IPv4 addresses can be categorized in Classes.
Classes define what part of an IPv4 address indicates the connected host and what part of the address indicates the network in which the host is connected to.
There are a total of 5 possible classes, identifiable by a letter ranging from A to E.

1. A
	* Ranges from 0.0.0.0 to 127.255.255.255
	* The first octet (the first 8 bits of the IP address) defines the network.
	* ```00000000|00000000.00000000.00000000```
	* Leading bits: 0000...
2. B
	* Ranges from 128.0.0.0 to 191.255.255.255
	* The first 2 octets (16 bits) define the network
	* ```10000000.00000000|00000000.00000000```
	* Leading bits: 1000...
3. C
	* Ranges from 192.0.0.0 to 223.255.255.255
	* 3 octets (24 bits) define the network and only 8 define the host.
	* ```11000000.00000000.00000000|00000000```
	* Leading bits: 1100...
4. D
	* 
	* Leading bits: 1110...
5. E
	*
	* Leading bits: 1111...

Classes can be identified by the "leading bits" when reading the IP in binary format.

---
## Subnet Masks

Subnet masks make the definition between host and network identifiers much more precise, which allows to create networks specifically made for ***anyone's*** needs.

## NAT

NAT is the base for local networks (LAN) as how we know it.


