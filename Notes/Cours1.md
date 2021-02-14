# Cours 1

### 1.1 What is the Internet?
- We'll talk about the basic hardware and software component that makes up the Internet
- In terms of networking infrastructure that provides services to distributed applications

#### 1.1.1 Nuts and Bolts Description
- It's a computernetwork that interconnects hundreds of millions of computing devices
- These devices are called **hosts**  or **end system**
- **End systems** are connected together by a network of **communication links**

```
Communication links: Coaxial cable, copper wire, optical fiber, radio spectrum
```

- Different links can transmit data at different rates.
- **Transmission rates** of a link is measure bits/second.
- When one end system has data to send to another end system, the sending end system segments the data and adds header bytes to each segment. 
- The resulting packages of information are called **packets**. 
- The packets are sent through the network to the destination end system, where they are reassembled into the original data.

- A packet switch takes a packet arrivng on one of its incoming communication links and forwards that packet on one of its outgoing communication links. 
- Packet switches comes in many shapes and flavors, but the two most prominent types are **routers** and **link-layer switches**
- Both types of switches forward packets to their ultimate destination
- Link-layer switches are typically used to access networks
- Routers are used in the network core
- The sequence of communication links and packet switches traversed by a packet from the sending end system to the receiving end system is known a **path** or a **route** through the network.


- End systems access the Internet through **Internet Service Providers (ISPs)**

```
ISPs:
Residential ISPs: Local cable, telephone companies;
Corporate ISPs; University ISPs; ISPs that provides WiFi access in airports, hotels, coffee shops, and other public places.
```

- Each ISP is in itself a network of packet switches and communication links.

```
ISPs provide a variety or types of network access to the end systems
Residential broadband access -> cable moden or DSL, hish-speed local area network access, wireless access, and 56 kbps dial-up modem access
Content Providers -> connecting websites directly to the Internet
```

- Internet is about connect end systems to each other, so the ISPs that provice access to end systems must also be interconnected. 
- Lower-tier ISP are interconnected through national and international upper-tier ISPs such as Level 3 Communications. **AT&T, Sprint, and NTT***

```
Upper-tier ISPs consists of high-speed routers interconnected with high-speed fiber-optic links.
```

- Each ISP network, whether upper-tier or lower-tier, is managed independently, runs the IP protocol, and conformed to certain naming and address convensions.
- End systems, packet switches, and other pieces of the Internet run **protocols** that control the sending and receiving of information within the Internet.
- The **Transmission Control Protocol (TCP)** and the **Internet Protocol (IP)** are two of the most important protocols in the Internet.

```
The Ip  protocol specifies the format of the packets that are sent and received among routers and end systems.
```

- The Internet's principal protocols are collectively known as **TCP/IP**. 
- **Internet Standards** ard developed by the **Internet Engineering Task Force (IETF)**.
- The IETF standards documents are called **requests for commets (RFCs).**
- RFCs define protocols such ad TCP, IP, HTTP (for the Web), and SMTP (for e-mail). 
- There are over 6,000 RFCs.
- The IEEE 802 LAN/MAN Standards Commiteee, specifies the Ethernet and wireless WiFi standards



