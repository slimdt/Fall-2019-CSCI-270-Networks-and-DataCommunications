# CSCI 270 
# Chapter 3: Addressing on Networks
## Objectives:
+ MAC address
+ TCP/IP
  - IP address
  - subnet mask
  - default gateway
  - DNS server
+ port and socket
+ domain names and name resolution process
+ command-lines tools for trouble-shooting
# Lecture 3 08/29/2019
## 4 addressing methods to locate the host/node on a network
+ **MAC address**
  - on data link layer
  - uniq for every NIC
  - 48 bits (00:60:8C:00:53:99)
  - used for nodes to find each other on a LAN
+ **IP** address
  - on network layer
  - assigned to nearly every **interface**(network connection made by a node)
  - used for routing
  - two types:
    + IPv4 (internet protocal version 4)
      - 32 bits, 4 decimal numbers called octets (192.168.0.1)
    + IPv6
      - 128 bits, 8 hexadecimal numbers (2001.0D88:0B80:0000:000000D3:9C5A:00CC)
+ **port** number
  - on transport layer
  - to find application
+ **FQDNs**: fully qualified domain name
  - on application layer
  - host name + domain name
  - for example `www.google.com` has a host name `www` and a domain name `google.com`
  - `blackboard.sau.edu` has a host name `blackboard` and a domain name `blackboard`
## MAC address
![](http://haslab.co.uk/images/MAC%20on%20NIC.png)
+ 48 bits/ 6 bytes (for example 00:60:8C:00:54:99)
+ OUI(organizationally unique identifier): first 24 bits (00:60:8C) and assigned by [IEEE(http://standards.ieee.org/regauth/oui/index.shtml)

+ extension identifier/device ID: last 24 bits

## IP address
+ static IP address
+ dynamic IP address by **DHCP**(dynamic Host Configuration Protocal) server
+ gateway: A computer/router/other device that a host uses to access another network. The default getway is a getway device that nodes on the network turn to first for access to outside world.
+ subnet mask/net mask
  - 32 bits 
  - seperate host ID from network ID (IP address consists of 2 parts, host ID and network ID)
+ DNS server
  - responsible for traching computer names and their IP addresses
+ You can use *ipconfig* utility in *Command Prompt* window  to find the current TCP/IP settings.

### IPv4
+ 32-bit/4 octets, the range of each octet (0,255)
+ the smallest IP 0.0.0.0, the laregest 255.255.255.255
+ the are totally 255*255*255*255 = 4.3 billion IPv4 addresses
+ IP = network ID(first 16 bits) + host ID(last 16 bits)
+ classful addression(5 classes: class A, class B, class C, class E, and class E)

|Class|Network octets|approximate number of networks|approximate num of IP addresses in each network|usage|
|----|----|----|----|---|
|A|1.x.y.z to 126.x.y.z|126|16 million|public|
|B|128.0.x.y to 191.255.x.y|16,000|65,000|public|
|C|192.0.0.x to 223.255.255.x|2 million|254|public|
|D|224.0.0.0 to 239.255.255.255|||multicast|
|E|240.0.0.0 to 254.255.255.255|||research|


|public IP address|private IP address|
|----|----|
|on the internet|on private network|
|class A,B,C|10.0.0.0 to 10.255.255.255<br>172.16.0.0 to 172.31.255.255<br>192.168.0.0 to 192.168.255.255|

**network portion and host porion for class A,B,C**
![](../Resources/ch3-classabc.png)

**reserved IP**
|IP address(es)|Function|
|----|----|
|255.255.255.255|broadcast,a broadcast message is read by every node on the network|
|0.0.0.0|currently unassigned|
|127.0.0.1 to 127.255.255.255|used for research or loopback address(your own computer IP)|
|169.254.0.1 to 169.254.255.254|used to create an APIPA(automatic private IP addressing) address when a computer configured for DHCP first connects to the network and is unable to lease an IPv4 address from the DHCP server|

## DHCP(dynamic host configuration protocal)
+ static IP addressing is usually unmanagable.
+


