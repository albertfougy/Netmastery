# Exploring the Functions of Networking

## What Is A Computer Network

> A computer network is a digital telecommunications network which allows nodes to share resources. - Wikipedia

A computer network can exist on its own, independent of other computer networks, and it can also connect to other networks. Globally speaking, the internet is an example of many interconnected networks.

Eons ago, the internet only connected several mainframe computers with computer terminals. The mainframe computers were large, and their computing power was considered enormous, although their computing power is equivalent to today's smartphones. The internet now connects not only laptops, smartphones, and tablets, but also IoT (Internet of Things) devices, TVs, game consoles, and much more. The earlier concept of centralized computing is revived today in the cloud.

Users who wish to connect their networks to the internet can acquire access through a service provider's access network. The service provider can use different technologies from dialup or broadband [telephony networks](https://en.wikipedia.org/wiki/Telephony), such as [ADSL networks](https://en.wikipedia.org/wiki/ADSL), cable networks, mobile, radio or fiber-optic networks. Service provider networks cover large geographical areas and connect with other providers for global coverage.

Computer networks can be classified in several ways, and then combined to find the most appropriate one for the implementation.

- **Distance**  
Between the user and the computer network the user is accessing, there is a distance that distinguishes the local and remote networks.

- **Purpose**  
Examples of networks categorized by their purpose would be data center networks and [SAN](https://en.wikipedia.org/wiki/Storage_area_network). Focusing on the technology used, you can distinguish between wireless or wired networks.

- **Size**  
Looking at the size of the network in terms of the number of devices it has, there are various types of networks. Such as small networks, usually with fewer than ten devices, medium to large networks consisting of tens to hundreds of devices, and very large, global networks, such as the internet, which connects thousands of devices across the world.  


- **Geographical Scope**  
        - **[LAN](https://en.wikipedia.org/wiki/Local_area_network)**  
  Local area networks connect devices located relatively close together in a limited area. An example would be a university campus network that can span several collocated buildings.<br/><br/>
  Enterprise networks often span across multiple locations, including a main office or Enterprise Campus and remote sites like branch offices or home offices of remote workers. **Small office, home offices (SOHO)**  typically only have a few devices and primarily connect to the main office network via the internet. The main office network is usually a Local Area Network (LAN) that may consist of multiple networks occupying multiple floors or a campus with several buildings. Wireless networks are often managed through **Wireless LAN Controllers (WLC)**, and most Enterprise Campuses have a separate data center to support business operations. Branch offices have their own LANs and resources such as printers and servers, but depend on the main office for operations and connect via a WAN or internet using routers.<br/><br/>**Intranet**

            - An intranet is a private computer network that uses internet technologies to securely share any part of an organization's information or operational systems within that organization. So, if the LAN is limited to internal use within an organization and is not accessible to the public, it can be referred to as an intranet. However, all intranets are LANs, but not all LANs are intranets.

    - **[WAN](https://en.wikipedia.org/wiki/Wide_area_network)**
      Wide area networks cover a broad geographical area and are managed by service providers. 

    - **[MAN](https://en.wikipedia.org/wiki/Metropolitan_area_network)**
      A computer network that interconnects users with computer resources in a geographic region of the size of a metropolitan area, such as a city.  

Enterprise networks are crucial to business activities, and they must be secure, resilient, and allow for growth. Network engineers often use validated network architecture models like the Cisco three-tier hierarchical network architecture model, the spine-leaf model, and the Cisco Enterprise Architecture model to assist in designing and implementing enterprise networks. These models provide hierarchical structure to enterprise networks in the form of layers such as LAN Access and LAN Core, which offer different functionalities.

![Cisco Enterprise Architecture Model](/Network-Fundamentals/images/cisco-enterprise-networks.png)
*Cisco Enterprise Architecture Model*  

### Protocols

Why do we need network protocols and standards?

Network protocols are a set of rules that define how devices communicate with each other in a network. These protocols include specifications such as signal voltage, allowable messages, message structure, lost message management, and error handling. They establish a common set of guidelines for all devices in a network, ensuring that information can be transmitted and received reliably and efficiently.

The need for network protocols arises from the fact that devices need an agreed-upon system of communicating, much like two people speaking the same language. Ethernet, for example, is a collection of network protocols and standards that serves as an example of such a system for network devices. Ethernet includes protocols for media access, packet structure, and error handling, which allows devices to communicate with each other in a standardized way.

Similarly, the internet follows a well-defined set of protocol rules, specifically designed for internet communication. These protocols dictate how data is transmitted between devices in networks and how devices communicate with each other. Industry-standard protocols are typically created by various networking or information technology organizations. Examples of such organizations include the Internet Engineering Task Force (IETF), the Institute of Electrical and Electronics Engineers (IEEE), and the International Organization for Standardization (ISO).

The internet is a global infrastructure composed of many computer networks that follow standardized communication rules. It supports various data exchange services, such as email or file transfers. The protocols and processes of the internet are defined in a set of documents called **[Request for Comments(RFCs)]( https://www.ietf.org/standards/rfcs/)**. These documents are maintained by the Internet Engineering Task Force and are freely available to the public. By following standardized protocols and processes, the internet allows devices and networks to communicate with each other in a reliable and efficient manner, making it one of the most important technological innovations of modern times.

***Internet vs. Web***  
            
            The words internet and web are often used interchangeably, but they do not share the same meaning. The internet is a global network that interconnects many networks and therefore provides a worldwide communication infrastructure. The World Wide Web describes one way to provide and access information over the internet using a web browser. It is a service that relies on connections provided by the internet for its function.

## Common Usage of Computer Network

Computer networks are built with one primary purpose—To enable communication.

- Communication between human beings, for example, two students communicating over a chat application on their phones to coordinate school work.
- Communication between network machines, for example, a humidity sensor communicating with a database to send the latest data.
- Communication between humans and machines, for example, when someone purchases movie tickets online.

### Understanding What Happens During Communication

Consider a scenario where two users, Alice and Bob, wish to communicate with each other via chat applications on their laptops. The application acts as a mediator between the user and the computer network, facilitating the transformation of the user's input into digital form represented by a series of ones and zeros or bits. This series can be quite lengthy, with each digit representing one bit of data. The digitalized information is then broken down into smaller groups by the application and computer's operating system, and prepared for transmission over the computer network.

Similar to people boarding a train, these groups of bits are grouped into smaller packets and assigned tags, such as priority tags, to indicate any special handling requirements. These packets are then transmitted as a digital signal through the computer network, encountering different network devices that help them navigate their way towards their destination.

The packets can take different paths depending on various characteristics such as the quality of the path and congestion. The network devices, such as the network switch and router, function like a train junction and stop respectively, steering the packets in the right direction.

Once the packets reach their destination, they are reassembled in their original sequence, converted back to their original form, and displayed by the chat application. For Alice and Bob to have a successful, real-time chat, Bob's computer must be powered on, connected to the network, and running the chat application. The computer network has protocols in place to prevent any issues that may arise during transmission to ensure the communication is successful, as is typically the case with network communication in our daily activities.

## Components of a Network

1. Router
2. Switch
3. Firewall
4. Server: A device that provides functions or services for a client.
5. Client: A client is a device that accesses a service made available by a server.<br/><br/>
*Servers and clients, also known as end hosts or endpoints, are remote computing devices that communicate bidirectionally with the connected network.*

![Network Components](/Network-Fundamentals/images/network-components.png)

Network Devices
Devices can be further divided into endpoints and intermediary devices:

- **Endpoints:** In the context of a network, endpoints are called end-user devices and include PCs, laptops, mobile phones, and smart home components. They can also include file servers, printers, sensors, and cameras. While end devices used to be physical hardware units, virtualization now allows for one physical device to emulate multiple end devices, optimizing resource utilization. In virtualization, the emulated computer system operates as a separate physical unit with its own operating system and software, using the host device's resources to perform its functions.

- **Intermediary devices:** These devices interconnect end devices or interconnect networks. In doing so, they perform different functions, which include regenerating and retransmitting signals, choosing the best paths between networks, classifying and forwarding data according to priorities, filtering traffic to allow or deny it based on security settings, and so on. As endpoints can be virtualized, so can intermediary devices or even entire networks. The concept is the same as in the endpoint virtualization—the virtualized element uses a subset of resources available at the physical host system. Intermediary devices that are commonly found in enterprise networks are:  

    - **Switches:** These devices enable multiple endpoints such as PCs, file servers, printers, sensors, cameras, and manufacturing robots to connect to the network. Switches are used to allow devices to communicate on the same network. In general, a switch or group of interconnected switches attempt to forward messages from the sender so it is only received by the destination device. Usually, all the devices that connect to a single switch or a group of interconnected switches belong to a common network and can therefore communicate directly with each other. If an end device wants to communicate with a device that is on a different network, then it requires "services" of a device that is known as a router, which connects different networks together.

    - **Routers:** These devices connect networks and intelligently choose the best paths between networks. Their main function is to route traffic from one network to another. For example, you need a router to connect your office network to the internet. An analogy that may help you understand the basic function of switches and routers is to imagine a network as a neighborhood. A switch is a street that connects the houses, and routers are the crossroads of those streets. The crossroads contain helpful information such as road signs to help you in finding a destination address. Sometimes, you might need the destination after just one crossroad, but other times you might need to cross several. The same is true in networking. Data sometimes "stops" at several routers before it is delivered to the final recipient. Certain switches combine functionalities of routers and switches, and they are called **Layer 3 switches**.

    - **APs:** These devices allow wireless devices to connect to a wired network. An AP usually connects to a switch as a standalone device, but it also can be an integral component of the router itself.

    - **WLCs:** These devices are used by network administrators or network operations centers to facilitate the management of many APs. The WLC automatically manages the configuration of wireless APs.

    - **Cisco Secure Firewalls:** Firewalls are network security systems that monitor and control the incoming and outgoing network traffic based on predetermined security rules. A firewall typically establishes a barrier between a trusted, secure internal network and another outside network, such as the internet, that is assumed not to be secure or trusted.

    - **Intrusion Protection System (IPS):** An IPS is a system that performs a deep analysis of network traffic while searching for signs that behavior is suspicious or malicious. If the IPS detects such behavior, it can take protective action immediately. An IPS and a firewall can work in conjunction to defend a network.

    - **Management Services:** A modern management service offers centralized management that facilitates designing, provisioning, and applying policies across a network. It includes features for discovery and management of network inventory, management of software images, device configuration automation, network diagnostics, and policy configuration. It provides end-to-end network visibility and uses network insights to optimize the network. An example of a centralized management service is the Cisco DNA Center.

![Network Breakdown](/Network-Fundamentals/images/network-components-breakdown.png)

## Characteristics of a Network

  - Topology:

  - Bitrate/Bandwidth:

  - Availability:

  - Reliability:
  
- Speed:

- Cost:

- Security:

- Quality of Service (QoS):

- Scalability:

## Physical vs. Logical Topologies

## Interpreting a Network Diagram

## Impact of User Applications on the Network

## Summary
