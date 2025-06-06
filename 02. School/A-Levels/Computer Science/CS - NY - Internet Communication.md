---
title: CS - NY - Internet Communication
category: A-Level
subject: Computer Science
topic: Networks
date: 2025-05-09
tags: [A-Level, Networks, Computer-Science, CS]
type: Lesson Note
---

> [!NOTE] Context/Summary
UNFINSHED

# Circuit Switching
- **Circuit Switching** involves creating a communication connection between two endpoints for the duration of a phone call or transfer of data
	- This does not work for the billions of inter-connected parts of the Internet which is why *Packet Switching* was developed - to allow a communications channel to be shared so that when one communication was temporarily not using it another could

# Data Packets
- When sending data across a network data is broken into *chunks* called **data packets** and assembled again at the receiving end
	- This increases *network efficiency* and *reliability*
## Packet Switching
- Packets are often sent across networks, *which are also often shared*, that have multiple connections with multiple routes through to a destination ![[Pasted image 20250509095839.png]]
## Routing
- Routers forward *data packets* from one network to another.
	- Each router stores data about the available routes to the destination node
	- Then looks up the destination IP address in its routing table to find the best router to forward the packet to
	- Each transfer between routers is known as a *hop*
	- Routers continue to forward the packet until it reaches its destination node
## Building a Packet
- At its core, a packet is a segment of data that needs to be sent, referred to as the *payload*
	- This part of the packet will often vary in size from 500-1500 bytes
	- Packets also include headers and trailers ![[Pasted image 20250509102941.png]]
- Packets are deliberately kept small to ensure that individual packets don't take excessive time to transfer, preventing other packets from moving
	- However, they can't be too small as it can make data transfer inefficient as unnecessary headers and trailers would be required and transferred each time
- The **Header** contains the recipient's address so that it can be directed appropriately across the network
	- Address of the sender is also included so replies can be sent appropriately
	- Packet Number and Overall Number of Packets in the transmission is attached to assist in reassembling the data
	- The *Time To Live* (TTL) or hop limit is also included ![[Pasted image 20250509103510.png]]
- The **Trailer** is added to the end of the packet
	- Contains *error checking components* that verify the data received in the payload has not been corrupted on transfer
	- Checksums and Cyclical Redundancy Checks (CRCs) are used to check the data by the receiving host
	- The same checksum is recalculated at the destination end
	- If they do not match, the data has become corrupted and is refused and a new copy is requested to be sent again

# What is a Protocol?
- A **Protocol** is a set of rules, or formal description, of the format of a digital transmission
	- e.g. It will cover the size of the packets, the contents and format of the header, the error detection and correction procedure
- **Gateways** are required where data is travelling from one network to another that uses different protocols
	- Header data is removed and reapplied using the correct format of the new network
	- A router and a gateway can often be combined into one integrated device
## Importance of Protocols and Standards
- A protocol defines a set of rules for data communication
- These must be standard across *all* devices in all networks in order for communication to work
	- The global standard suite of networking protocols currently is **TCP/IP**
# TCP/IP Protocol Stack
- The **TCP/IP** stack is a set of rules used in turn to format a message so it can be sent over a network
	- Each layer provides a specific function within the transmission of the message ![[Pasted image 20250519150146.png]]
- **TCP/IP** uses *four connected layers* to allow network communication to take place
- Each layer wraps the packets with its own *header data*
	- Application Layer
	- Transport Layer
	- Internet Layer
	- Link Layer
### Application Layer
- This layer is used to provide services for applications that want to communicate across a network, *often the Internet*
	- Uses high-level protocols that set an agreed standard between the communicating end-points
	- For example, FTP for File Transfer and HTTP for Web Browsing
	- Doesn't determine how data is transmitted, rather specifies the rules of what should be sent
- e.g. a webpage is requested by a client computer so a .png web image is to be requested from a web server by the client browser using HTTP
### Transport Layer
- Uses the **Transmission Control Protocol (TCP)** to establish an end-to-end connection with the recipient computer 
	- Splits data into packets and numbers them sequentially
	- Adds port number to be used based on HTTP protocol
	- At the receiving end, this layer confirms that packets have been received and requests any missing packets be resent ![[Pasted image 20250519150818.png]]
### Internet Layer
- Uses the **Internet Protocol (IP)** to address packets with the source and destination IP addresses
	- A router forwards each packet towards an endpoint called a socket, defined by the combination of the IP address and port number ![[Pasted image 20250519151318.png]]
### Link Layer
- This layer operates across a physical connection
	- Adds the MAC address of the physical NIC that packets should be sent to based on the destination IP address
	- MAC addresses change with each hop ![[Pasted image 20250519151425.png]]
## Media Access Control Addresses (MAC Addresses)
- A MAC address uniquely identifies a physical device with a NIC
	- e.g. *4B:24:A2:73:0E:F1*
	- May be the destination computer or a router in transit
	- Packets move up and down the lower layers of the stack as they hop across routers, changing their source and destination MAC addresses as they go
## Port Numbers
- A port is used to alert a specific application to deal with data sent to a computer
- Several common application level protocols use standard ports: ![[Pasted image 20250519151742.png]]
# Related Notes
[[CS - NY - Networks & Web Technologies]]