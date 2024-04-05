## Types of network

- LAN: Local area network, e.g. a building.
- WAN: Wide area network, e.g. a city, a country, or the internet itself.

## Network devices

- Hub: Broadcasts info to every device on the network.
- Switch: Makes connections between specific devices, only sends data where needed.
- Router: Connects multiple networks together.
- Modem: Connects a router to the internet.

So an example flow is device -> router -> modem -> internet -> modem -> router -> device

## Virtualization tools

- Software that performs network operations, instead of physical hardware.

## Network models

![](files/tcpip-vs-osi-models.png)

### TCP/IP model

- TCP: Transmission Control Protocol, protocol allowing devices to form a connection and stream data.
- IP: Internet Protocol, set of standard for routing and addressing data packets.

1. Network access layer (Ethernet, WLAN): Creating data packets, transferring within network. Includes all hardware.
2. Internet layer (IPv4/6): Where IP addresses are added, connecting between networks.
3. Transport layer (TCP, UDP): Control flow of traffic, error control, permitting connections, etc.
4. Application layer (HTTP, DNS): How the data packets will interact with receiving devices.

### OSI model

1. Physical layer: All the low level hardware.
2. Data link layer: Sending and receiving data packets in-network.
3. Network layer: Transferring packets between networks, handling packet structure.
4. Transport layer: Transferring packets between devices, error handling, speed of transfer.
5. Session layer: Handles all the session-related logic.
6. Presentation layer: Encryption, data confirmation, character encoding.
7. Application layer: Data handled by programs, e.g. a web browser.

## IPv4 packet

![](files/ipv4-packet.png)

## IPv4 vs IPv6 header

![](files/ipv4-vs-ipv6.png)

## Feedback

A very dense module! Lots of good information, explained effectively. A great refresher of comp sci at uni.
