## 1.2 The Network Edge

- They are called end systems because they sit at the edge of the Internet.

The Internet end systems include: Desktop computers (desktop PCs, Macs, and Linux boxes), servers (Web and e-mail servers), and mobile computers (laptops, smartphones, and tablets).
- End systems are also referred to as *hosts* because they host (run) application programs such as a Web browser program, a Web server program, an e-mail client program, or an e-mail server program.

host = end system

Hosts are sometimes further divided into two categories: **clients** and **servers**

Clients: desktop and mobile PCs, smartphones, and so on.
Servers: More powerful machines that store and distribute Web pages, stream video, relay e-mail, and so on

- Most servers today from which we receive, search results, e-mail, Web pages, and video reside in a large **data centers.**

ex: Google has 30-50 data centers with many having more than one hundred thousand servers

### 1.2.1 Access Networks

- Let's consider the access network, the network that physically connects an end system to the first router (also known as the "edge router") on a path from the end system to any other distant end system.

#### Home Access: DSL, Cable, FTTH, Dial-Up, and Satellite

- Two of the most prevalent types of broadband residential access are **digital subscriber line (DSL)** and cable
- A residence typically obtains DSL Internet access from the same local telephone company (telco) that provides its wired local phone access.
- When DSL is used, a customer's telco is also its ISP
- Each customer's DSL modem uses the existing telephone line (twisted-pair copper wire) to exchange data with a digital subscriber line access multiplexer (DSLAM) located in the telco's local central office (CO).
- The homes DSL takes digital data and translates it to high-frequency tones for transmission over telephone wires to the CO; the analog signals from many such houses are translated back into digital format at the DSLAM
- Residential telephone line carries both data and traditional telephone signals simultaneously, which are encoded at different frequencies:
  - A high-speed downstream channel -> in the 50kHz to 1MHz band
  - A medium-speed upstream channel -> in the 4 kHz to 50 kHz band
  - An ordinary two-way telephone channel -> in the 0 to 4kHz band

This approach makes the single DSL link appear as if there were three separate links, so that a telephone call and an Internet connection can share the DSL link at the same time.

- On the customer side, a splitter separates the data and telephone signals arriving to the home and forwards the data signal to the DSL modem. 
- On the telco side, in the CO, the DSLAM separatesthe data and phone signals and sends the data into the Internet

Hundreds or even thousands of households connect to a single DSLAM 

- The DSL standards define transmission of 12 Mbps downstream and 1.8 Mbps upstread, and 24 Mbps downstream and 2.5 Mbps upstream.
- Because the upstream and downstream rates are different, the access is said to be assymetric.
- The actual upstream and downstream transmission rates achieved may be less than the rate noted above, as the DSL provider may purposefully limit residential rate when tiered service (different rates, available at different prices) are offered, or because the maximum rate can be limited by the distrance between the home and the CO, the gauge of the twisted-pair line and the degree of electrical interference. 
- Generally, if the residence is not located within 5 to 10 miles of the CO, the residence must resort to an elternative form of Internet access,

While DSL makes use of telco's existing local telephone infrastructure, **cable Internet access** makes use of the cable television company's existing cable television infrastructure.
- Aresidence can obtain cable Internet access from the same company that provides its cable television.
- Fiber optics connect the cable head end to neighbourhood-level junctions, from which traditional coaxial cable is then used to reach individual houses and appartments. 
- Each neighbourhood junction typically supports 500 to 5,000 homes.
- Because both fiber and coaxial cable are employed in this system, it is often referred to as hybrid fiber coax (HFC) p.14

- Cable internet access requires special modems, called cable modems.
- As with a DSL modem, the cable modem is typically an external device and connects to the home PC through an Ethernal port.
- At the cable head end, the cable modem termination system (CMTS) servers a similar function as the DSL network's DSLAM - turning the analog signal sent from the cable modems in many downstream homes back into digital format.
- Cable modem divide the HFC network into two channels, a downstream and a stream channel. 

- As with DSL, access is typically asymmetric, with the downstream channel typically allocated a higher transmission rate than the upstream channel.
- The DOCSIS 2.0 standard defines downstream rates up to 42.8 ,bps and upstream rates of up to 30.7 Mbps
- As in the case of DSL networks, the maximum achievable rate may not be realized due to lower contracted data rates or media impairments.

- One important characteristic of cable Internet access is that it is a shared broadcast medium. In particular, every packet sent by the head end travels downstream on every link to every home and every packet send by a home travels on the upstream channel to the head end (Headend = is the facility at a local cable TV).
- For this reason, if several users are simultaneously downloading a video file on the downstream channel, the actual rate at which each user receives its video file will be significantly lower than the aggregate cable downstream rate.
- On the otehr hand, if there are only a few active users and they are all Web surfing, then each ofthe users may actually receive Web pages at the full cable downstream rate, because the users will rarely request a Web page at exactly the same time. 
- Because the upstream channel is also shared, a distributed multiple access protocol is needed to coordinate transmissions and avoid collisions.

- Although DSL and cable networks currently represent more than 90 percent of residential broadband access in the US, and up-and-coming technology that promises even higher speeds is the deployment of **fiber to the home (FTTH)** 
- As the name suggests, the FTTH concept is simple-provide an optical fiber path from the CO directly tot he home.
- In the US, Verizon has been particularly aggressive with tthe FTTH WITH ITS fios SERVICE (2012)

- There are several competing technologies for optical distribution from the CO to the homes.
- The simplest optical distribution network is called direct fiber, with one fiber leaving the CO for each home.
- More commonly, each fiber leaving the central office is actually shared by many homes.; it is not until the fiber gets relatively close to the homes that it splits into individual customer-specific fibers. There are two competing optical-distribution network architectures that perform this splitting: active optical networks (AONs) and passive optical networks (PONs).
- AON is essentially switched Ethernet.
- PON: Each home has an optical network terminator (ONT), which is connected by dedicated optical fiber to a neighborhood splitter.
- The splitter combines a number of homes (typically less than 100) onto a single, shared optical fiber, which connects to an optical line terminator (OLT) in the telco's CO.

### 1.2.2 Physical Media

- A physical medium can take many shapes and forms and does not have to be of the same type for each transmitter-receiver pair along the path.
ex: twisted-pair copper wire, coaxial cable, multimode fiber-optic cable, terrestrial radio spectrum, and satellite radio spectrum.

Physical medium fall into two categories:
- Guided media and unguided media

Guided media: the waves are guided along a solid medium -> fiber-optic cable, twister-pair copper wire, or a coaxial cable
Unguided media: the waves propagate in the atmosphere and in outer space, such as in wireless LAN or a digital satellite channel

- Cost of physical link (copper wire, fiber-optic, etc) is often relatively minor compared with other networking cost.
- Labot cost associated with the installation of the physical link can be orders of magnitude higher than the cost of the material.
- For this reason, many builders install twisted-pair, optical fiber, and coaxial cable in every room in a building even if only one medium is initially used. There is a good chance that another medium could be used in the near future, and so money is saved by not having to lay additional wires in the future.

#### Twisted-pair copper wire
- The least expensive and most commonly used guided transmission medium.
- For hundreds of years, it has been used by telephone networks.
- More than 99% of the wired connections from the telephone handset to the local telephone switch use twisted-pair copper wire.
- Twisted pair consists of two insulated copper wires, each about 1mm thick, arranged in a regular spiral pattern.
- The wires are twisted together to reduce the electrical interference from similar pairs close by. 
- - A wire pair constitute a communication link

**Unshielded twisted pair (UTP)** is commonly used for computer networks within a building, that is for LANs.
