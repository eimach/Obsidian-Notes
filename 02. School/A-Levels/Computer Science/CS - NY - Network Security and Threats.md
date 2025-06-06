---
title: CS - NY - Network Security and Threats
category: A-Level
subject: Computer Science
topic: Networks
date: 2025-05-19
tags: [A-Level, CS, Computer-Science]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# Firewalls
- The entrance to a network can be protected in the same way
	- A **firewall** is either software or hardware that controls access to and from a network
	- Ports are opened so that only certain traffic is allowed to pass through
## Packet Filtering 
- Data packets are inspected by the firewall to check which port they are attempting to access
- Different network protocols use different port numbers for example, HTTP uses port 80 or 8080
	- If this traffic is to be allowed through, the port must be opened for the duration of the connection, otherwise the firewall will automatically reject it
## Proxy Server
- Proxy servers make web requests on behalf of your own computer, hiding the true request IP addresses from the recipient
- Functions of a **Proxy Server**:
	- Enables anonymous surfing
	- Filter undesirable online content
	- Log user requests
	- Provides a cache of previously visited sites to speed access
## Encryption
- The act of encoding a plaintext message so that it cannot be deciphered unless you have a numerical key to decrypt it
# Malicious Software
- Malware annoys users or damages their data
## Worms
- A worm is a standalone program that does not require a user to run it in order for it to spread
- Worms exploit vulnerabilities in the destination system and spread automatically
## Trojans
- Trojans are malicious software programs that imitate useful applications
- Cannot self-replicate
- Serve to open up backdoors in your computer to the Internet so that the processing power, bandwidth and data can be exploited remotely
## Phishing
- Is using emails to manipulate a victim into visiting a fake website and giving away personal information
# Code Quality
- Improving **code quality**, together with monitoring attempts to gain unauthorised access and protection can significantly reduce threats from malware
- Includes:
	- Guarding against *Buffer Overflow* attacks
	- Guarding against *SQL Injection* attacks
	- Use of strong passwords for login credentials
	- Two-Factor Authentication
	- Use of Access Rights (File System Permissions)
# Common Attacks
- There are two common attacks:
	- SQL Injection
	- Buffer Overflow
## SQL Injection
- A malicious user can enter SQL commands via online database forms to change the processing
	- e.g. If used on a banking website, it can produce the SQL to display the account details
## Buffer Overflow
- Buffer Overflow occurs when a program accidentally writes data to a location too small to handle it 
- As a result, the overflowed *data* may end up in neighbouring *instruction* space
- Malware can deliberately cause and manipulate overflow data which may then be read as a malicious '**instruction**' 

# How to Protect from Threats?
- **Monitoring** and **Prevention** are some ways of protecting from threats
	- Monitoring: Using *Packet Sniffers* and *User Access Logs*
	- Prevention: Up-to-Date Patches and Updates for the OS and applications reduce vulnerabilities, 
# Related Notes
[[Computer Science MOC]]
[[CS - NY - Networks & Web Technologies]]