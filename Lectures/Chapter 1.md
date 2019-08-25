# CSCI 270 Fall 2019
# Lecture 1 08/22/2019
## Why should we learn this course?
1. Core courses of CS:
+ Computer Organization and Architecture
+ Data Structures and Algorithms
+ Operating Systems
+ Fundamentals of Compiling
+ **Computer Networks**
2. Waves of technologis
+ Search Engine
+ Big Data
+ Cloud Computing
+ AI
+ BlockChain

For the architecture of any big system, good **network** -> half done.
**Computer Networks** is foundation of many new technologies.


# Chapter 1: Introduction Networking

## Objectives
+ client-server vs. peer-to-peer networks
+ types of applications and protocols
+ hardware devices and physical topologies
+ seven-layer OSI model
+ safety and trouble-shooting

# Q: What is a network?
## network
  + hardware devices
  + topologies
  + protocols 

## hardware devices
For example?

## topologies
+ physical topologies (hardware)
Devices fit together to form a network.
+ logical topologies (software: operating system)
   + peer-to-peer(P2P)
  OS of each computer controls its own adiministrations, resources and security without a centralized control. The computers are also connected directely.
  ![p2p example](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/P2P-network.svg/1200px-P2P-network.svg.png)
    - advantages:
    1. easy to set up
    2. not expensive
    - disadvantages:
    1. not scalable: not easy to add more devices to the network
    2. not practical for 15 computers
   + client-server
  controlled by NOS via a centralized directory database
  **domain**: computers/clients controlled by the server
  **AD(active directory)**: the centralized directory database
  **AD DS(domain service)**:: manages clients' getting accesss to server
  ![client-server example](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/Client-server-model.svg/1200px-Client-server-model.svg.png)
     - advantage
      1. user account and password
      2. resources sharing
      3. problems are easy to fix
      4. more scalable
### applications vs. protocals
  + protocals are agreements.
  + applications follow protocals.
  
  #### Protocals: 
  A protocal consists of 
  1. syntax：  in some specific format.
  2. semantic: meaningful.
  3. sequence: in order.
  Only throught protocals, a group of computers can colaborate to complete a huge task.
  #### Examples
  1. Data transmission: TCP, UDP, IP
  2. Web service: HTTP, HTTPS (for both server and client)
  3. Email service: SMTP (for client), POP3, IMAP4 (for server)
  4. FTP service: FTP (client-server)
  5. Telnet/remote control service: telnet(client-server)
  6. ...
  **Protocals in OSI seven-layer model**
  ![oso protocals](https://blogs.bmc.com/wp-content/uploads/2018/06/osi-model-7-layers-1024x734.jpg)
  
  
             
  #### Characteristics of protocals:
  1. too many to remember
  2. You feel you understand some protocal, but you can not explain it clearly.
  3. You do not know how to solve practical problems.
  #### Procedure of learning  protocals:
  1. You feel you know it once you learn it
  2. You feel overwhelmed when being asked questions
  3. You feel frustrated in real projects.
  
  #### How to learning Computer Networks/Protocals?
  1. use daily examples
  2. use CISCO Packet Tracer
  [CISCO Packet Tracer: download and training course](https://www.netacad.com/courses/packet-tracer)
  
  3. imagine you are "there"
  
# CSCI 270 Fall 2019
# Lecture 2 08/27/2019

  ## Network Hardware
  ### LANs(Local Area Network) and their hardware
  ![LAN example](https://www.learnabhi.com/wp-content/uploads/2018/02/LAN.jpg)
  #### topologies
  **ring topology**(legacy topology, barely used today)![ring](https://cdn.comparitech.com/wp-content/uploads/2018/11/Ring-Topology.jpg)
  **star topology**![star topology](https://2.bp.blogspot.com/-ehAbcPHrS4g/WE183W2IqbI/AAAAAAAAArg/L2-OXyLpLG4bkCq6Oyi5k4adtEdUkbtowCLcB/s1600/Star-topology.png)
  
  **mesh topology** ![mesh](https://cdn.comparitech.com/wp-content/uploads/2018/11/Mesh-Topology.jpg)
  
  **bus topology** ![bus](https://cdn.comparitech.com/wp-content/uploads/2018/11/Bus-Topology.jpg)
  
  
  **hybrid topology** ![hybrid](https://1.bp.blogspot.com/-cF4N0TPUg-8/V7HuNumKVII/AAAAAAAAAIg/4ZPBrd67NDo2Jf9B0zrKTfVA7X4dN766ACLcB/s1600/hybrid%2Btopology.png)
  
  #### hardware
  1. Hub(legacy device)
  2. Switch
  
  **compare hubs and switches in CISCO Packet Tracer**
  3. Network Port(where you plug your network cable)
    + on motherboard
    + on NIC(network interface card)
    
  
  
  


      
  
  


