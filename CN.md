# Introduction

## Computer Network

A Computer Network is a group of computers connected with each other through wired or wireless medium, such that they can exchange information.

### Components

There are six basic components of a Computer Network:

1. **Node**: A Computer or a device in a network that participates in data sending or receiving
2. **Link**: A connection between any two nodes. Can be wired, or wireless
3. **Message**: The data that is being sent in a network
4. **Sender**: The *Node* that sends the data in a network
5. **Receiver**: The *Node* that receives the data.
6. **Protocol**: A set of rules agreed to by both sender and receiver which helps in establishing a reliable communication between the two.

### Features

A computer network has the following features:

1. **Performance:** The response time of sending and receiving data from one node to another should be minimal.

2. **Data Sharing:** Nodes should be able to share data between different systems connected with each other through a transmission media.

3. **Backup:** It must have a central server that keeps the backup of all the data that is to be shared over a network so that in case of a failure it should be able to recover the data faster. 

4. **Software and hardware compatibility**: A computer network should allow better compatibility between different software and hardware configurations.

5. **Reliability:** There should not be any failure in the network, or if it occurs the recovery from a failure should be fast. 

6. **Security:** A computer network should be secure so that the data transmitting over a network should be safe from unauthorized access. Also, the sent data should be received as it is at the receiving node, which means there should not be any loss of data during transmission.

7. **Scalability:** A computer network should always allow adding new computers (or nodes) to the already existing computer network.

### Applications

1. Resource Sharing
2. Information Sharing
3. Communication
4. Entertainment Industry
5. Access to Remote Databases
6. Home applications
7. Business applications
8. Mobile users
9. Social media


# Terminology

## Protocol

A protocol is a *set of rules and standards* that govern how data is transmitted over a network. Examples of protocols include TCP/IP, HTTP and FTP.

## Topology

Network topology refers to the physical and logical *arrangement of nodes* on a network. The common network topologies include bus, star, ring, mesh and tree.

### Mesh Topology

Here, every device has a dedicated point-to-point link to every other  device. The term dedicated means that the link carries traffic only between the two devices it connects.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.netadmintools.com%2Fwp-content%2Fuploads%2FMesh-Network-Topology.png&f=1&nofb=1&ipt=6a11fd297b274c5243c2e0afcefba0dc0e91d95df20f2ab885760b073f646738&ipo=images" height = 400>

To find the number of physical links in a fully connected mesh network with `n` nodes:

- Every node `i` must be  connected to `n - i` nodes.
- So we need `n(n - 1)` physical links.
- If each physical link allows communication in both directions (duplex mode), we can divide the number of links by 2.
- Thus we can say that we need `n(n - 1) / 2` duplex links.
- Every device on the network must have `n - 1` I/O ports to be connected to the other `n - 1` stations.  

#### Pros

- Use of dedicated links: Each connection can carry its own data load, thus eliminating traffic problems.
- Robust: If one link becomes unusable, it does not incapacitate the entire system.
- Privacy or security. When every message travels along a dedicated line, only the intended recipient sees it.
- Point-to-point links make fault identification and fault isolation easy. Traffic can be routed to avoid links with suspected problems.

#### Cons

The main disadvantages of a mesh are related to the amount of cabling and the number of I/O ports required.

- Because every device must be connected to every other device, installation and re-connection are difficult.
- The sheer bulk of the wiring can be greater than the available space (in walls, ceilings, or floors) can accommodate.
- The hardware required to connect each link (I/O ports and cable) can be prohibitively expensive. 

For these  reasons a mesh topology is usually implemented in a limited fashion, for example, as a backbone connecting the main computers of a hybrid network that can include several other topologies. 

#### Applications

One practical example of a mesh topology is the connection of telephone regional offices in which each regional office needs to be connected to every other regional office.

### Star Topology

In a star topology, each device has a dedicated point-to-point link only to a central controller, usually called a hub. The devices are not directly linked to one another. Unlike a  mesh topology, a star topology does not allow direct traffic between devices. The controller acts as an exchange: If one device wants to send data to another, it sends the data to the controller, which then relays the data to the other connected device.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.itrelease.com%2Fwp-content%2Fuploads%2F2019%2F06%2FStar-topology-diagram-1024x819.png&f=1&nofb=1&ipt=f383f30185fe6562e91cc2c3ee718d5566846eac366c4cae3b433fd3e3eee8ff&ipo=images" height = 400>

#### Pros

- Less expensive than a mesh topology.
- Each device needs only one link and one I/O port to connect it to any number of others.
- Far less cabling needs to be housed.
- Additions, moves, and deletions involve only one connection: between that device and the hub.
- If one link fails, only that link is affected. All other links remain active.
- Easy fault identification fault isolation.

#### Cons

- Dependency of the whole topology on one single point, the hub: If the hub goes down, the whole system is dead.
- More cabling is required in a star than in some other topologies (such as ring or bus).

#### Applications

The  star topology is used in local-area networks (LANs)

### Bus Topology

The preceding examples all describe point-to-point connections. A bus topology, on the other hand, is multipoint. One long cable acts as a backbone to link all the devices in the network.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F3.bp.blogspot.com%2F-6OyWTyAxQ20%2FWqfJSnK10FI%2FAAAAAAAAASM%2FTDYbNHk5fBMtJ_euRESlTGnS0q1C7zh4ACLcBGAs%2Fs1600%2Fbus.png&f=1&nofb=1&ipt=651e69754cb917b0ab555b7916a108e448cb56396c61c986aa8e3fa2f3c6d3b4&ipo=images" height = 400>

Nodes are connected to the bus cable by drop lines and taps.

- A **drop line** is a connection running between the device and the main cable.
- A **tap** is a connector that either splices into the main cable or punctures the sheathing of a cable to create a contact with the metallic core.

As a signal travels  along the backbone, some of its energy is transformed into heat. Therefore, it becomes weaker and  weaker as it travels farther and farther. For this reason there is a limit on the number of taps a bus can support and on the distance between those taps.

Bus topology was the one of the first topologies used in the design of early local area networks.
#### Pros

- Ease of installation. Backbone cable can be laid along the most efficient path, then connected to the nodes by drop lines of various lengths.
- Less cabling than mesh or star topologies.

#### Cons

- Difficult re-connection and fault isolation.
- Difficult to add new devices.
- Signal reflection at the taps can cause degradation in quality.
- A fault or break in the bus cable stops all transmission, even between devices on the same side of the problem.

#### Applications

Ethernet LANs can use a bus topology, but they are less popular now.

### Ring Topology

In a ring topology, each device has a dedicated point-to-point connection with only the two devices on either side of it. A signal is passed along the ring in one direction, from device to device, until it reaches its destination. Each device in the ring incorporates a repeater. When a device receives a signal intended for another device, its repeater regenerates the bits and passes them along

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimages.wevolver.com%2FeyJidWNrZXQiOiJ3ZXZvbHZlci1wcm9qZWN0LWltYWdlcyIsImtleSI6ImZyb2FsYS8xNjI0NjEzNjg4OTczLVJpbmctVG9wb2xvZ3kgKDEpLnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6OTUwLCJmaXQiOiJjb3ZlciJ9fX0%3D&f=1&nofb=1&ipt=84b20c7de232bf98d2cd917bb11e807a38aa6489829c3c79c403492ceb359483&ipo=images" height = 400>

#### Pros

- Relatively easy to install and reconfigure.
- Each device is linked to only its immediate neighbors (either physically or logically).
- To add or delete a device requires changing only two connections. The only constraints are media and traffic considerations (maximum ring length and number of devices). 
- Fault isolation is simplified. 
  Generally in a ring, a signal is circulating at all times. If one device does not receive a signal within a specified period, it can issue an alarm. The alarm alerts the network operator to the problem and its location.

#### Cons

- A break in the ring can disable the entire network.

#### Applications

Ring topology was prevalent when IBM introduced its local-area network Token Ring. Today, the need for higher-speed LANs has made this topology less popular.

### Hybrid Topology

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimages.wevolver.com%2FeyJidWNrZXQiOiJ3ZXZvbHZlci1wcm9qZWN0LWltYWdlcyIsImtleSI6ImZyb2FsYS8xNjI0NjEzMzM5MjI2LUh5YnJpZC1Ub3BvbG9neS5wbmciLCJlZGl0cyI6eyJyZXNpemUiOnsid2lkdGgiOjk1MCwiZml0IjoiY292ZXIifX19&f=1&nofb=1&ipt=c0773f419037d9c75b0ff506207a57349ea6b0071fbfef1b9803d3a34888c82c&ipo=images" height = 400>

A network can be hybrid. For example, we can have a main bus topology with each branch connecting several stations in a star topology.

## IP Address

An IP address is a *unique numerical logical identifier* that is assigned to every device on a network. IP addresses are used to identify devices and enable communication between them.

## DNS

The Domain Name System (DNS) is a *protocol* that is used to translate human-readable domain names (such as www.google.com) into IP addresses that computers can understand.

## Firewall

A firewall is a *security device* that is used to monitor and control incoming and outgoing network traffic. Firewalls are used to protect networks from unauthorized access and other security threats.

## Simplex

In simplex mode, the communication is *unidirectional*, as on a one-way street. Only one of the two devices on a link can transmit; the other can only receive. Keyboards and traditional monitors are examples of simplex devices.

## Half-Duplex  

In half-duplex mode, each station can *both transmit and receive*, but *not* at the *same time*. When one device is sending, the other can only receive, and vice versa. Walkie-talkies are half-duplex systems.  

## Full-Duplex  

In full-duplex, *both stations can transmit and receive simultaneously*. One common example of full-duplex communication is the telephone network. When two people are communicating by a telephone line, both can talk and listen at the same time. The full-duplex mode is used when communication in both directions is required all the time.

## Types of Networks

|                        |         **PAN**         |      **LAN**       |               **CAN**                |          **MAN**          |       **WAN**        |
| ---------------------- | :---------------------: | :----------------: | :----------------------------------: | :-----------------------: | :------------------: |
| **Full Name**          |  Personal Area Network  | Local Area Network |         Campus Area Network          | Metropolitan Area Network |  Wide Area Network   |
| **Technology**         | Bluetooth, IrDA, Zigbee |  Ethernet, Wi-Fi   |               Ethernet               |      FDDI, CDDI, ATM      | Leased Line, Dial-Up |
| **Range**              |       1 m - 100 m       |       < 2 Km       |             1 Km - 5 Km              |       5 Km - 50 Km        |       > 50 Km        |
| **Transmission Speed** |        Very High        |     Very High      |                 High                 |          Average          |         Low          |
| **Area**               |      Within a Room      |  Within Building   | Within University, Corporate offices |        Within City        |   Within Countries   |
| **Ownership**          |         Private         |      Private       |               Private                |     Private or Public     |  Private or Public   |
| **Maintenance**        |        Very Easy        |        Easy        |               Moderate               |         Difficult         |    Very Difficult    |
| **Error rate & Cost**  |        Very Low         |        Low         |               Moderate               |           High            |      Very High       |

# Reference Models

## OSI Model

- OSI -> Open System Interconnection
- It is a model for designing a network architecture that is flexible, robust and interoperable.
- Developed by ISO - International Standards for Organisations.
- Has 7 layers:
<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Finsights.profitap.com%2Fhs-fs%2Fhubfs%2FThe%25207%2520Layers%2520of%2520OSI.png%3Fwidth%3D560%26name%3DThe%25207%2520Layers%2520of%2520OSI.png&f=1&nofb=1&ipt=e495cebc35be8aa4dbb9af2a03ac5cd1f160d524eb52c6ee3694b7944a7806c8&ipo=images" height = 400>

1. **Physical Layer**
	- Last layer in Sender side, First layer in Receiver side
	- Deals with hardware, i.e. physical devices:
		- Topologies
		- Cables, Connectors etc.
		- Hubs, Repeaters, Routers etc.
	- Deals with Signal type and Signal Transmission method

2. **Data Link Layer**
	- Deals with:
		- Errors when they are detected in this flow
		- How long a node should be allowed to transmit or receive data
		- How much data should be allowed to transmit
	
	- Uses **MAC** address -> Media Access Control:
		- MAC Address is a unique hardware identification number.
		- This is given to a device at the time of manufacture. 
		- It lives on NICs (Network Interface Cards)

3. **Network Layer**
	- Deals with:
		- Communications between Nodes or Networks or both
		- Uses IP addresses
		- **Routers** specialize in this layer as they facilitate this functionality

4. **Transport Layer**
	- Deals with:
		- Line Discipline, Flow control, Error control
		- Data packet segmentation
	
	- Transport layer also has understanding of message. So it can control flow by not sending the whole message at a time, and hence reduce network congestion.

5. **Session Layer**
	- A **Session** is a connection established between two specific end-user applications. So this layer establishes, maintains and terminates sessions.

6. **Presentation Layer**
	- Deals with:
		- Data formatting, such as character encoding and conversions
		- Data encryption
	
	- This layer makes sure that end-user applications operating here can successfully consume data and display it.

7. **Application layer**
	- This is the topmost layer, responsible for supporting services used by end-user applications.
	- Protocols working in this layer include:
		- File Transfer Protocol (FTP)
		- Secure Shell (SSH)
		- Simple Mail Transfer Protocol (SMTP)

## TCP/IP Model

- TCP/IP -> Transmission Control Protocol / Internet Protocol
- Developed prior to OSI model
- Developed by ARPANET
- Unlike OSI model, TCP/IP is actually implemented
- Has 4 / 5 layers:
<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.mevspace.com%2Fen%2Fstatic%2F83c05c5fac51fd68cd8938dbd408db61%2Fa94c1%2Ftcp-ip-model.png&f=1&nofb=1&ipt=c4c293e0c313c41dd3f461ede6fc76020279c0725d5d9e40ef18ccaddb7cafc6&ipo=images" height = 600>
- The *Network Interface layer* is sometimes split up just like OSI model into:
	- Data layer
	- Physical layer

# Transmission medium

A transmission medium can be broadly defined as anything that can carry information from a source to a destination.

## Terminology

### Twisted-Pair Cable

A twisted pair consists of two conductors (normally copper), each with its own plastic insulation, twisted together. One of the wires is used to carry signals to the receiver, and the other is used only as a ground reference.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.pngkit.com%2Fpng%2Ffull%2F815-8153857_unshielded-twisted-pair-png.png&f=1&nofb=1&ipt=9014a675924c7bc7f44c6fe8e126dc4de4155150805a43918613b3242bfa37ad&ipo=images" width = 400>

The most common twisted-pair cable used in communications is referred to as **Unshielded twisted-pair** **(UTP)**. **Shielded twisted pair** **(STP)** cable has a metal foil or braided mesh covering that encases each pair of insulated conductors. Although metal casing improves the quality of cable by preventing the penetration of noise or cross-talk, it is bulkier and more expensive.

The most common UTP connector is **RJ45** (RJ stands for *registered jack*)

#### Applications

Twisted-pair cables are used in:
- telephone lines to provide voice and data channels.
- Local-area networks, such as `10Base-T` and `100Base-T`, also use twisted-pair cables.

### Coaxial Cable

Coaxial cable (or _coax_) carries signals of higher frequency ranges than those in twisted pair cable. Coax has a central core conductor of solid or stranded wire (usually copper) enclosed in an insulating sheath, which is, in turn, encased in an outer conductor of metal foil, braid, or a combination of the two. The outer metallic wrapping serves both as a shield against noise and as the second conductor, which completes the circuit. This outer conductor is also enclosed in an insulating sheath, and the whole cable is protected by a plastic cover.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.topcable.com%2Fwp-content%2Fuploads%2F2020%2F12%2FTOP-CABLE-COAXIAL-DIGITAL-cobre.png&f=1&nofb=1&ipt=f3cc6457ad6d87a1a1d5f75f2aadef96ac922c180e2aa16c6138a4b434e260c3&ipo=images" height = 400>

The most common type of connector used today is the **Bayone-Neill-Concelman (BNC)** connector.

#### Applications

Coaxial cable was widely used in:
- Analog telephone networks
- Digital telephone networks
- Cable TV networks also use coaxial cables.
- Traditional Ethernet LANs

## Fiber-Optic Cable

A fiber-optic cable is made of glass or plastic and transmits signals in the form of light. Light travels in a straight line as long as it is moving through a single uniform substance. If a ray of light traveling through one substance suddenly enters another substance(of a different density), the ray changes direction.

Optical fibers use reflection to guide light through a channel. A glass or plastic core is surrounded by a cladding of less dense glass or plastic.

#### Propagation Modes

1. **Multi-mode** is so named because multiple beams from a light source move through the core in different paths.
2. **Single-Mode** uses step-index fiber and a highly focused source of light that limits beams to a small range of angles, all close to the horizontal.

In **multi-mode step-index fiber**, the density of the core remains constant from the center to the edges. A beam of light moves through this constant density in a straight line until it reaches the interface of the core and the cladding. The term _step index_ refers to the suddenness of this change, which contributes to the distortion of the signal as it passes through the fiber.

A second type of fiber, called **multimode graded-index fiber**, decreases this distortion of the signal through the cable. The word _index_ here refers to the index of refraction.

#### Fiber Connectors

- **Subscriber channel** (SC) connector
- **Straight-tip** (ST) connector
- **MT-RJ(mechanical transfer registered jack)** connector

#### Applications

- Fiber-optic cable is often found in backbone networks because its wide bandwidth is cost-effective.
- Some cable TV companies use a combination of optical fiber and coaxial cable,thus creating a hybrid network.
- Local-area networks such as `100Base-FX` network (Fast Ethernet) and `1000Base-X` also use fiber-optic cables.

#### Advantages

- *Higher bandwidth*
- *Less signal attenuation*. Fiber-optic transmission distance is significantly greater than that of other guided media. A signal can run for 50 km without requiring regeneration. We need repeaters every 5 km for coaxial or twisted- pair cable.
- *Immunity to electromagnetic interference*. Electromagnetic noise cannot affect fiber-optic cables.
- *Resistance to corrosive materials*. Glass is more resistant to corrosive materials than copper.
- *Light weight*. Fiber-optic cables are much lighter than copper cables.
- *Greater immunity to tapping*. Fiber-optic cables are more immune to tapping than copper cables. Copper cables create antenna effects that can easily be tapped.

#### Disadvantages

- *Installation and maintenance*
- *Unidirectional light propagation*. Propagation of light is unidirectional. If we need bidirectional communication, two fibers are needed.
- *Cost*. The cable and the interfaces are relatively more expensive than those of other guided media. If the demand for bandwidth is not high, often the use of optical fiber cannot be justified.

# Wireless



# Network Devices



# Switching

## Message Switching

## Circuit Switching

## Packet Switching

