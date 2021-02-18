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
- -Fiber optics connect the cable head end to neighbourhood-level junctions, from which traditional coaxial cable is then used to reach individual houses and appartments. 
- Each neighbourhood junction typically supports 500 to 5,000 homes.
- Because both fiber and coaxial cable are employed in this system, it is often referred to as hybrid fiber coax (HFC) p.14

