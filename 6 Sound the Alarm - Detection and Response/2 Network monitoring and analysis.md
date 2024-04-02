## Network

- IoC: Indicators of compromise, observable evidence that there may have been a security incident
- Data exfiltration: Unauthorized transmission of data from a system
- Network _traffic_: Amount of data that moves across network.
- Network _data_: The data itself.

## Monitoring

- Flow analysis: Monitoring if any unusual ports / packets / protocols are in use.
- Packet payload info: Orgs might look inside packets at the actual data.
- Temporal patterns: Is data transferred inside typical working hours?

## Defensive measures

- Prevent attacker access
- Monitor network activity
- Protect assets
- Detect and stop exfiltration

## Packet captures

"P-cap": Packet capture (unnecessary term, eh?)

Can come in following formats (copied verbatim):

1. **Libpcap** is a packet capture library designed to be used by Unix-like systems, like Linux and MacOS®. Tools like tcpdump use Libpcap as the default packet capture file format.
2. **WinPcap** is an open-source packet capture library designed for devices running Windows operating systems. It’s considered an older file format and isn’t predominantly used.
3. **Npcap** is a library designed by the port scanning tool Nmap that is commonly used in Windows operating systems.
4. **PCAPng** is a modern file format that can simultaneously capture packets and store data. Its ability to do both explains the “ng,” which stands for “next generation.”

## IP packet details

### IPV4

- Version: v4/6
- Internet Header Length: Length of header + options
- Type of Service: Priority
- Total Length
- Identified, Flags, Fragment Offset: Fragment = packet has been split into chunks, info on how to reassemble.
- Time To Live: How long until drop
- Protocol: E.g. tcp = 6
- Header checksum
- Source & destination address
- Options is sometimes used for debugging etc
- Finally, the actual data!

### IPV6

- Version
- Traffic class: Similar to type of service
- Flow label: Identifies if from specific source(?)
- Payload length
- Next header(?)
- Hop limit: Similar to TTL
- Source & destionation address

## tcpdump

`sudo tcpdump -i any -v -c 1`

- sudo: Need to run as superuser.
- tcpdump: Duh, want to use tcpdump.
- -i any: Interface to sniff on (any).
- -v: Verbose
- -c 1: Count, capture 1 packet
