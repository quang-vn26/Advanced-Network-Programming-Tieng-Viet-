**Chapter 2**
**Network Architectures**

Abstract The networks have evolved significantly since the first network architecture has been proposed. Lately, the architecture is seen more as a framework which specifies not only the network topology, network type, network components,
and their functionality, but also presents data communication protocols, data formats used, and supported services. This chapter introduces network topologies, network types, and network components, and discusses several network communication technologies.

**2.1 Introduction**

|                                                              |      |
| ------------------------------------------------------------ | ---- |
| Designing network architectures and proposing or improving various data communication protocols were at the center of extensive research and development interest. Various network architectures have been proposed since 1950s when the first architecture involving several communication links only used to connect central processors to remote peripherals (e.g., printers). The networks have evolved significantly since, and currently a network architecture is seen as a framework which specifies not only network topology, network type, network components, and their functionality, but also presents data communication protocols available, data formats employed, and a set of services supported. Often billing aspects are also considered. |      |
| The first two chapters of this book discuss network architectures and data communication protocols focusing on two directions. This chapter details network<br/>topologies, types, components, and communications technologies, and the next<br/>chapter presents communication protocols and services, respectively. |      |
| Network components include many network devices which enable data exchange<br/>between different network parts alongside end-user devices. Network topologies<br/>indicate how network devices are interconnected by links and how all these are<br/>arranged to form a functional communication network. When discussing network<br/>types, one refers to the classification of networks based on various aspects, including<br/>size, communication technology, etc., and when mentioning network components,<br/>the focus is on both network links and network devices. Communication technologies are concerned with the mechanisms employed to exchange data between interconnected network or user devices via the communication links, whereas protocols<br/>are seen as formal mechanisms to exchange messages between network components. A protocol architecture includes all the protocols used to transport messages<br/>over a certain network infrastructure and indicates the way these protocols interact<br/>with each other. Although there is a thin line separating services from protocols, the<br/>latter are seen mostly application-linked and related to the network interface with<br/>end-users or devices. |      |
| All these aspects are of extreme importance for application developers, especially<br/>when performance constraints are involved. This chapter introduces network architectures’ major aspects with the focus on existing and future network technologies. |      |
|                                                              |      |
|                                                              |      |

**2.2 Network Topologies**





|                                                              |      |
| ------------------------------------------------------------ | ---- |
| A network topology refers to the arrangement of nodes (i.e., network devices,<br/>servers, and host machines) and links between them to form a computer network.<br/>Nowadays, various types of topologies have been proposed and are in use. Among<br/>these topologies, most known are ring, star, bus, tree, mesh, and ad-hoc. These will<br/>be discussed in detail next. |      |

**2.2.1 Ring Topology**

![image-20200903213537384](/home/quangg/.config/Typora/typora-user-images/image-20200903213537384.png)

|                                                              |      |
| ------------------------------------------------------------ | ---- |
| In a ring topology, each node is connected with exactly two other nodes forming<br/>a single data path in a form of a ring. Such a network arrangement is presented in<br/>Fig. 2.1. |      |
| In the basic ring network topology, the messages (data bits) travel in one direction<br/>only. Each node has a dual role, as a host and as a relay. As a host, each node will<br/>send data messages to other nodes and will receive messages addressed to it. As a<br/>relay, each node forwards messages addressed to other nodes to the next node on<br/>the ring. |      |
| The main issue concerning ring networks is their reliability. If a single link is<br/>broken, the communication between certain nodes is impeded. Dual ring solutions,<br/>where communication is possible both clockwise and anticlockwise, have been proposed to improve reliability through redundancy. The increase in redundancy comes<br/>with higher deployment and maintenance costs. |      |
| Standardization related to the ring topology includes the Token Ring protocol<br/>(IEEE 802.5), initially proposed by IBM. Apart from the specifications of the protocol, IEEE 802.5 also includes details on the data formats. |      |

**2.2.2 Star Topology**

![image-20200903213620259](/home/quangg/.config/Typora/typora-user-images/image-20200903213620259.png)

|                                                              |      |
| ------------------------------------------------------------ | ---- |
| In a star topology, every host is connected to a central network component (denoted<br/>as hub), which may be a network hub, a switch, or a router, as illustrated in Fig. 2.2. |      |
| This topology is very popular for home networks where various devices such as<br/>desktop PCs, laptops, and mobile devices are connected to a local router, which is<br/>further connected to the broadband modem. |      |
| In terms of link failure, star topologies are more robust. If a certain link fails, only<br/>the hosts using those links will be disconnected from the network, while all the other<br/>hosts will not experience any disruptions in communications. The negative aspects<br/>of a star topology include the existence of a single point of failure and increased deployment costs. The latter has been mitigated with the latest advancements in<br/>wireless networking. |      |
|                                                              |      |

**2.2.3 Bus Topology**

![image-20200903214029004](/home/quangg/.config/Typora/typora-user-images/image-20200903214029004.png)