# Routers
Routing happens on the Third layer of [[#The ISO/OSI model]]. The router receives data packages from a device on the network and then decides to what router send it next or to directly send it to the destination if it's on the local network, this is done through the IP and Port and with specially made routing protocols and [[#routing tables]]. An example routing protocol is **dixtra**'s algorithm, which was written to paper in the early 80s.

Emulators: cisco packet tracer; gns3
## The ISO/OSI model
The International Standard Organization/Open Systems Interconnection protocol model is formed by 7 layers that standardize communications between devices.
The layers are:
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application
Bitches added two sublevels tho:
1. LLC (Makes packages to ship to MAC)
2. MAC (Machine Access Control)
These adapt stuff from the top (check on book)
## The TCP/IP Protocol
The TCP/IP protocol is an implementation of [[#The ISO/OSI model]] that groups the 7 layers into 4 which are the following:
1. Application (layers 7 and 6)
   Uses protocols such as Telnet, FTP, SMTP
2. Transport (layers 5 and 4)
   Uses protocols such as TCP and UDP
3. Network (layer 3)
   Uses protocols such as ICMP and IGMP (IP)
4. Link (layers 2 and 1)
   It's related to the Network Interface Cards and their relative drivers.
## Routing Tables
Routing tables are made by the router by pinging every so often other routers to share it's own current status and get that router's status.

# Subnet Masks
- Subnet mask for class A: 255.0.0.0
- Subnet mask for class B: 255.255.0.0
- Subnet mask for class C: 255.255.255.0
Those zeroes can also be other values. In the case those aren't zeroes it means that the LAN has been partitioned into subnets.
## Particular notation for subnet masks
- Class A is /8
- Class B is /16
- Class C is /24

209.10.20.0
255.255.255.224  /27

| Network Address | Broadcast Address |
| :-------------- | :---------------- |
| `209.10.20.0`     | `209.10.20.31`      |
| `209.10.20.32`    | `209.10.20.63`      |
| `209.10.20.64`    | `209.10.20.95`      |
| `209.10.20.96`    | `209.10.20.127`     |
| `209.10.20.128`   | `209.10.20.159`     |
| `209.10.20.160`   | `209.10.20.191`     |
| `209.10.20.192`   | `209.10.20.223`     |
| `209.10.20.224`   | `209.10.20.255`     |

## Logical and Physical topology
The logical structure describes how data transits in the physical topology.
Page 8 standards table.
IEEE 802.


