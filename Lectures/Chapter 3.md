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
+ OUI(organizationally unique identifier): first 24 bits (00:60:8C) and assigned by (IEEE)[http://standards.ieee.org/regauth/oui/index.shtml]

  
      
