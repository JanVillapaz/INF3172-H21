### 1.1.2 A Service Description

Internet *as an infrastructure that provides services to applications*

Applications such as : electronic mail, Web surfing, social networks, instant messaging, Voice-over-IP (VoIP), 
video streaming, distributed games, peer-to-peer (P2P) file sharing, television over the internet, remote login, and etc.

- The application are said to be **distributed applications** since they involve multiple end systems that exchange data with each other.
- Internet applications run on end systems - they do not run on packet switches in the network core.

- Packet systems facilitate the exchange of data among end systems, they are not concerned with the application that is the source or sink of data

- An infrastructure that provides services to application: Imagine having a great idea for a distributed internet application.
How to transform this idea into an actual Internet application? Because applications run on end systems, you would need to write programs that run on the end systems. (Write in Java, C, or Python.) Now because it is a distributed Internet Application, the programs running on different end systems will need to send data to each other. (Leads to the alternative way of describing the Internet as a platform for applications). 
- How does one program running on one end system instruct the Internet to deliver data to another program running on another end system?
- End systems attached to the Internet provide an **Application Programming Interface (API)** that specifies how a program running on one end system asks the Internet infrastructure to deliver data to a specific destination program running on another end system. 

- The Internet API is a set of rules that the sending program must follow so that the Internet can deliver the data to the destination program. 

**Two descriptions of Internet talked about so far**
Internet in terms of:
- hardware and software components
- infrastructure for providing services to ditributed applications

### 1.1.3 What is a Protocol?

#### Network protocols

- Entities exchanging messages and taking actions are hardware or software components of some device (ex: computer, smartphone, tablet, router, or other network-capable device).
- All activities in the Internet that involves two or more communicating remote entities is governed by a protocol. 

ex: hardware-implemented protocols in two physically connected computers control the flow of bits on the "wire" between the two network interface cards; 
congestion-control protocols in end systems control the rate at which packets are transmitted between sender and receiver; 
protocols in routers determine a packet's path from source to destination.

ex of a computer network protocol:
consider what happens when you make a request to a Web server, that is when you type a URL of a web page into your Web browser.
1. The computer will send a connection request message to the Web server and wait for a reply
2. The web server will eventually receive your connection request message and return a connection reply message
3. Knowing it is OK to request the Web document, your computer then send the name of the Web page it wants to fetch from that Web server in a GET message
4. Finally, the Web server returns the Web page (file) to your computer. 

Exchange of messages and the actions taken when these messages are sent and received are the key defining elements of a protocol.

``
A protocol defines the format and the order of messages exchanged between two or more communicating entities, as well as the actions taken on the transmission and/or receipt of a message or other event.
``

- Different protocols are used to accomplish different communication tasks.

