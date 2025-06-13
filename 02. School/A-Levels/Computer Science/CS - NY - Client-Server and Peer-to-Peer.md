---
title: CS - NY - Client-Server and Peer-to-Peer
category: A-Level
subject: Computer Science
topic: Networks
date: 2025-06-13
tags: [A-Level, CS, Computer-Science, Networks]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Client-Server
- Consists of two part: *Client* and *Server*
	- The **Client** accesses data, services and files from the *Server*
	- **Client** initialises communications to the server
	- The *Server* waits for requests from **Clients**
	- Terminals are known as '*clients*' of the central server![[Pasted image 20250613092654.png]]
## Networking of Client-Servers
- Features of a client-server network include:
	- Central Server to manage security
	- Some files are held on the Central Server
	- Some processing tasks are performed by the server
	- Clients issue requests to the server for services such as email, file storage, backup and printing
	- Can require specialist IT staff to administer the network
# Peer-to-Peer
- Peer-to-Peer has **no** *central server*
- Features include:
	- They are suitable for a small company or home network with a few computers
	- No central server controls files or security
	- All computers can see files on all other computers
	- All computers can communicate with each other without going through server
	- If a computer is switched off, data cannot be retrieved from it
# Summary of the Architectures

| Client-Server                                              | Peer-to-Peer                                                           |
| ---------------------------------------------------------- | ---------------------------------------------------------------------- |
| User IDs, passwords and access levels centrally controlled | Files and programs stored on individual computers                      |
| Used in many small, medium-size and large organisations    | Suitable for a home computer network                                   |
| Can be expensive to set up and to manage                   | Cheap to set up and maintain                                           |
| Backup is centralised and usually automated                | Each computer on the network can act as both client and server         |
| No access to other users' files                            | Can be used for sharing of music and streaming coverage of live events |

# Client Processing
- Clients include desktops, tablets, phones, consoles, etc...
	- Data is processed *before* it is sent to a server by the **client**
	- On the web, this usually happens in the form of scripts and these are usually executed by the client browser
	- The web page does not communicate with the server at this point
## Use of JavaScript
- Web pages may feature *JavaScript* to validate data before it gets sent to the server for further validation

| Advantages                                                                          | Disadvantages                                                                                                                                    |
| ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Allows for more interactivity by immediately responding to a users' action          | Not all browsers support all scripts (although most modern browsers support an overwhelming majority)                                            |
| Quick execution as no communication with the server is required                     | Because the scripts are processed by the client, they are dependent on the performance of the clients' machine                                   |
| Removes potentially unnecessary processing from the server                          | Different browsers process scripts in slightly different ways, so the web page owner cannot be certain how the end-product will look to the user |
| Data cannot be intercept on the way to the server, increasing security for the user |                                                                                                                                                  |
## Client Side Processing
- Scripts that handle initial processing saves the server valuable processing resources
- If all of the terminals in this network had to communicate each time they needed to validate information, the server would eventually become overloaded and would crash
### Application Programming Interface (API)
- APIs are a set of tools that can be used for building software applications
- API requests are processed by the client and responded to by the relevant server, such as Google Maps
## Server Side Processing
- In certain cases, it is necessary for a server to process information to:
	- Process User Input -> Another layer of validation
	- Display Pages
	- Structure Web Applications
	- Interact with Permanent Storage/Databases using SQL
- Server Programming Languages include:
	- Python
	- PHP
	- ASP
- The client does not always have the capability to provide the data required to successfully process a request
- A company may hold sensitive data relating to the request
- The way the data is processed may also be a company secret and be protected by law, such as Google PageRank
- A server may wish to further validate data that has been submitted by the client
	- This may have already been validated on the client-side using JS but JS can be easily circumvented
	- This makes additional server-side validation crucial to accurate, secure data being transmitted
- For example, this is how client processing and server processing works on the Argos website ![[Pasted image 20250613100622.png]] ![[Pasted image 20250613100750.png]]

# Related Notes
[[CS - NY - Networks & Web Technologies]]