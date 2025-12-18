# CHAPTER 11: Networking & Distributed Systems

This chapter covers how computers communicate and work together.

## 1. The OSI and TCP/IP Models
Conceptual models for networking protocols.
- **OSI (7 Layers)**: Physical, Data Link, Network, Transport, Session, Presentation, Application.
- **TCP/IP (4 Layers)**: Network Interface, Internet, Transport, Application.
  - The TCP/IP model is the practical standard used for the Internet.

## 2. Protocols (HTTP, DNS, UDP)
- **HTTP/HTTPS (HyperText Transfer Protocol)**: The foundation of data communication for the World Wide Web. Stateless, request-response model.
- **DNS (Domain Name System)**: The phonebook of the internet. Translates human-readable domain names (google.com) to IP addresses.
- **TCP (Transmission Control Protocol)**: Reliable, ordered, error-checked delivery. Connection-oriented.
- **UDP (User Datagram Protocol)**: Connectionless, faster, but unreliable. Used for streaming and gaming.

## 3. Client-Server vs. Peer-to-Peer
- **Client-Server**: Centralized model. Clients request resources; servers provide them. Easier to manage and secure but the server is a single point of failure and bottleneck.
- **Peer-to-Peer (P2P)**: Decentralized. Each node acts as both client and server (peers). Highly scalable and robust (e.g., BitTorrent) but harder to manage.

## 4. Latency, Bandwidth, and Throughput
- **Bandwidth**: The maximum capacity of the channel (how wide the pipe is).
- **Latency**: The time it takes for a packet to travel from source to destination (the delay).
- **Throughput**: The actual rate of data transfer achieved.
- "You can't fix latency with bandwidth."
