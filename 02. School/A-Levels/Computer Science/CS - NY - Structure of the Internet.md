---
title: CS - NY - Structure of the Internet
category: A-Level
subject: Computer Science
topic: Networks
date: 2025-03-25
tags:
  - A-Level
  - Networks
  - CS
  - Computer-Science
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Connecting Computers
- Computers communicate with each other through the use of **networks**
	- The largest public network is the Internet, which is known as a *Wide Area Network* (*WAN*)
- Similar to a road network, data traffic is directed to any location if the destination address is known
# Structure of the Internet
- The main part of the Internet is known as the backbone
	- This is a set of dedicated connections that connect several large networks at various points on the globe
	- Each of these points are connected to other regional networks, usually controlled by *Internet Service Providers* (*ISPs*) which provide access to individual end-users
# Internet Addresses
- Each device on a network needs to be uniquely identified so data can be sent to the correct destination
	- This is done through the *Internet Protocol* addressing system
## IP Addressing
- IP Version 4 (*IPv4*) addresses are made up of **4** *octet* values (*numerical values described by 8 bits*) separated by a full-stop
	- e.g. *14.132.250.10* or *230.197.1.192* or *127.0.0.1*
	- Has a range from 000.000.000.000 -> 255.255.255.255
	- The address is divided into a *Network* portion and a *Host* portion; the division is determined by the *subnet mask*
		- The first *3* octets are the Network Portion -> *192*.*168*.*0*.x
		- The last octet is the Host Portion -> xxx.xxx.xxx.*24*
		- A 192.168.1.1/24 -> /24 = Network is First 3 Octets, Host is the last Octets
		- **Can make a separate note on the IP classes of own learning and go more in-depth**
- There is also *IPv6* addresses as there were not enough IPv4 addresses
## Uniform Resource Locator
- URLs are used to specify the means of accessing a resource across a network and its location
- The protocol and the domain name of the resource form the URL
	- "*http://*" - specifies that the resource requires http (webpage)
	- *"www.bbc.co.uk/index.html"*  - the fully qualified domain name and name of the resource to be accessed (*index.html*)
	- The URL is the combination of the two
## Domain Name System (DNS)
- DNS servers are dedicated computers with an index of domain names and their corresponding IP addresses.
	- When a computer queries a DNS server for a domain name, the server returns an IP address that the computer can use to send a message to
	- e.g. *www.google.co.uk* -> 216.58.209.99
### DNS Server Structure
- There are 13 root DNS servers that work together to catalogue every domain name ![[Pasted image 20250325151716.png]]
## Resolving an IP Address
1. Find bbc.co.uk - domain name is resolved from right to left
2. Local DNS doesn't know - refers to root
3. Root may know or knows where .uk server is
4. Refers to .co server
5. Find BBC server and resolves IP address
6. Returns IP address
![[Pasted image 20250325152842.png]]
- If a client has no cached record of an IP address for www.google.co.uk, it sends a DNS query for that domain to its specified DNS server
- If the DNS server does not have a record for that domain, it will either:
	- recursively handle the request so that it can eventually deliver an IP address or a "DNS address could not be found" error message
	- or refer to a DNS server authoritative, e.g. *.uk*, and follows this, and subsequent referrals, to successively lower-level DNS servers

## Internet Registries
- Domain names must be unique otherwise DNS requests could beconfused
- There are *5* global **Internet Registries** responsible for allocating IP addresses to specific domain names
	- They work together to maintain a database of address assignments to ensure an IP is used once and domain names are distinct
	- These are www.arin.net, www.ripe.net, www.lacnic.net, www.afrinic.net, www.apnic.net 

# Local Area Networks (LANs)
- One computer, not connected to any other computing device is called a *standalone*
- Once multiple computers are connected, a network is formed and fall into one of two categories:
	- **Local Area Network** (LAN)
	- **Wide Area Network** (WAN)
- A **LAN** is *two or more computers connected together within a small georaphical area, e.g. a building or site*
![[Pasted image 20250328103945.png]]

# Network Topologies
- Is the arrangement of various computing devices which make up a computer network
- There are *2* types of **Topologies**:
	- Bus Topology: an arrangement where nodes are connected in a daisy chain by a single centre communications channel
	- Star Topology: an arrangement where a central node or hub provides a common connection point for all other nodes

## Bus Network
![[Pasted image 20250328104903.png]]
- All nodes are connected to a single backbone cable
- Each end of the backbone is connected to either a terminator or a computer which stops signals 'bouncing back'
- Each node is passive
- Data is sent in on direction at a time only
- Only one computer can transmit successfully at any one time
- **Advantages**:
	- Inexpensive to set up
	- Devices can easily be added
	- Good for small networks
- **Disadvantages**:
	- Main cable is a point of failure
	- Limited cable length
	- Performance degrades with heavy use -> owing to data collision
	- Poor Security
## Star Network
![[Pasted image 20250328110051.png]]
- Computers are connected to a central node which is often a *1*
- **Advantages**:
	- Easy to isolate problems
	- Good performance
	- More secure if a switch is used as data is only sent to the recipient
- **Disadvantages**:
	- Can be expensive to set up because of the length of cable required
	- Central device is a point of failure

## Physical vs Logical Topology
- **Physical** Topology defines how the devices are physically connected
- **Logical** Topology defines how the devices communicate across physical topologies
	- e.g. a network wired in star topology can heave logically as a bus network

# Purpose of Wi-Fi
- Wi-Fi is a wireless networking technology providing high-speed internet and network connections
- Devices connect to the Internet via a *Wireless Access Point* (WAP)
- Some Wireless Components are:
	- Wireless Network Interface Card (NIC)
	- A *Station* consists of a computer and a *NIC*
	- Stations share a *radio frequency channel*
	- A *WAP* requires a connection to a router which requires a connection to a modem
		- *WAP and Modem are often built into the router*
# Related Notes
[[Computer Science MOC]]
[[CS - NY - Networks & Web Technologies]]