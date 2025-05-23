# Routing-and-Switching

## 1. Switching
### Definition:
Switching is the process of forwarding data within a local area network (LAN) using MAC addresses. It allows devices on the same network to communicate efficiently.

### Device Involved:
Switch – A Layer 2 device (Data Link Layer) that connects devices in a LAN.

![Routing-and-Switching](https://tse4.mm.bing.net/th?id=OIP.GwZIzkJbMBtB2wHR3ZbMtAHaDW&pid=Api&P=0&h=220)

### How Switching Works:
Each device connected to a switch has a unique MAC address.

The switch maintains a MAC address table (or CAM table) that maps MAC addresses to its ports.

When a frame arrives, the switch:

Reads the destination MAC address.

Looks it up in the MAC table.

Forwards the frame to the correct port.

## Types of Switching:
Circuit Switching – A dedicated path is established (used in telephone networks).

Packet Switching – Data is broken into packets and sent individually (used in computer networks).

Message Switching – Whole messages are stored and forwarded (rarely used today).

### Switching Methods:
Store-and-Forward – Entire frame is read, checked for errors, then forwarded.

Cut-Through – Switch forwards as soon as the destination MAC is read.

Fragment-Free – Starts forwarding after first 64 bytes (reduces errors).

### Advantages of Switching:
Efficient LAN communication

Reduces collisions

Supports full-duplex

Increases bandwidth

## 2. Routing
### Definition:
Routing is the process of forwarding data between different networks using IP addresses.

### Device Involved:
Router – A Layer 3 device (Network Layer) that connects multiple networks.

### How Routing Works:
Routers use IP addresses to determine the destination network of a packet.

They consult their routing table to find the best path to the destination.

The router then forwards the packet to the next hop or final destination.

## Types of Routing:
Static Routing – Manually configured routes.

Dynamic Routing – Routes learned automatically via routing protocols.

Default Routing – A catch-all route used when no specific route is found.

### Common Routing Protocols:
RIP (Routing Information Protocol) – Distance-vector, max hop count 15.

OSPF (Open Shortest Path First) – Link-state, fast and scalable.

EIGRP (Enhanced Interior Gateway Routing Protocol) – Cisco proprietary.

BGP (Border Gateway Protocol) – Used on the Internet between ISPs.

### Functions of a Router:
Determine best path using metrics (hop count, bandwidth, delay).

Perform Network Address Translation (NAT).

Provide firewall and security features.

Segment broadcast domains.

