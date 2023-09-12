# Routers
Routing happens on the Third layer of [[#The ISO/OSI model]]. The router receives data packages from a device on the network and then decides to what router send it next or to directly send it to the destination if it's on the local network.
## The ISO/OSI model
The International Standard Organization/Open Systems Interconnection protocol model is formed by 7 layers that standardize communications between devices.
The layers are:
1. Physical
2. Data Link
3. N(etwork?)
4. Transport
5. Session
6. P(rotocol?)
7. Application
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
