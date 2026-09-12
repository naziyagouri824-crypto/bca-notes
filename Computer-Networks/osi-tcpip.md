# OSI Model, TCP/IP & Switching

## 1. Layering in Computer Networks

Layering is a technique in which network communication is divided into different layers.

Each layer performs a specific function and communicates with the layer above and below it.

### Advantages of Layering

- Makes network design easier
- Reduces complexity
- Makes troubleshooting easier
- Allows different technologies to work together
- Each layer can be developed independently

---

# 2. OSI Model

OSI stands for **Open Systems Interconnection**.

The OSI model is a reference model developed by ISO for understanding how data is communicated between different devices over a network.

The OSI model has **7 layers**.

### Seven Layers of OSI Model

1. Application Layer
2. Presentation Layer
3. Session Layer
4. Transport Layer
5. Network Layer
6. Data Link Layer
7. Physical Layer

### Easy Way to Remember

**A P S T N D P**

Application → Presentation → Session → Transport → Network → Data Link → Physical

---

# 3. Application Layer

The Application Layer is the topmost layer of the OSI model.

It provides network services directly to the user applications.

### Functions

- Provides network services to applications
- Enables communication between network applications
- Supports services such as web browsing and email

### Examples

- HTTP
- HTTPS
- FTP
- SMTP
- DNS

---

# 4. Presentation Layer

The Presentation Layer is responsible for the format and representation of data.

### Functions

- Data translation
- Data encryption and decryption
- Data compression and decompression

### Example

It can convert data into a format that the receiving system can understand.

---

# 5. Session Layer

The Session Layer manages sessions between two communicating devices.

### Functions

- Establishes a session
- Maintains a session
- Terminates a session
- Provides synchronization

### Example

A session between a client and a server during communication.

---

# 6. Transport Layer

The Transport Layer provides reliable data transfer between devices.

### Functions

- Segmentation of data
- Error control
- Flow control
- Reliable delivery
- End-to-end communication

### Examples

- TCP
- UDP

---

# 7. Network Layer

The Network Layer is responsible for delivering packets from source to destination across different networks.

### Functions

- Logical addressing
- Routing
- Packet forwarding

### Example

IP addresses are used at this layer.

### Example Protocol

- IP

### Device

- Router

---

# 8. Data Link Layer

The Data Link Layer provides reliable communication between directly connected devices.

### Functions

- Framing
- Error detection
- Physical addressing
- Flow control

### Device

- Switch
- Bridge

### Example

MAC address is used at this layer.

---

# 9. Physical Layer

The Physical Layer is the lowest layer of the OSI model.

It deals with the physical transmission of bits through the communication medium.

### Functions

- Transmission of bits
- Defines cables and connectors
- Defines electrical and physical signals
- Controls data transmission over the physical medium

### Examples

- Twisted pair cable
- Coaxial cable
- Optical fiber

---

# 10. OSI Layers Summary

| Layer | Name | Main Function |
|---|---|---|
| 7 | Application | Network services to applications |
| 6 | Presentation | Translation, encryption, compression |
| 5 | Session | Session management |
| 4 | Transport | Reliable data delivery |
| 3 | Network | Routing and logical addressing |
| 2 | Data Link | Framing and MAC addressing |
| 1 | Physical | Transmission of bits |

---

# 11. TCP/IP Model

TCP/IP stands for **Transmission Control Protocol / Internet Protocol**.

It is a practical networking model used for communication over the Internet.

The TCP/IP model commonly has **4 layers**.

### Four Layers of TCP/IP Model

1. Application Layer
2. Transport Layer
3. Internet Layer
4. Network Access Layer

---

# 12. Application Layer of TCP/IP

The Application Layer provides network services to user applications.

It combines the functions of the OSI:

- Application Layer
- Presentation Layer
- Session Layer

### Examples

- HTTP
- HTTPS
- FTP
- SMTP
- DNS

---

# 13. Transport Layer of TCP/IP

The Transport Layer provides communication between applications running on different devices.

### Main Protocols

### TCP

TCP stands for **Transmission Control Protocol**.

It provides reliable and connection-oriented communication.

### UDP

UDP stands for **User Datagram Protocol**.

It provides faster but connectionless communication.

---

# 14. Internet Layer

The Internet Layer is responsible for delivering packets between networks.

### Main Functions

- Logical addressing
- Routing
- Packet delivery

### Main Protocol

- IP

Routers mainly work with this layer.

---

# 15. Network Access Layer

The Network Access Layer is responsible for communication over the physical network.

It combines functions related to:

- Data Link Layer
- Physical Layer

### Examples

- Ethernet
- Wi-Fi
- Network cables

---

# 16. OSI vs TCP/IP

| OSI Model | TCP/IP Model |
|---|---|
| 7 layers | 4 layers |
| Reference model | Practical networking model |
| Developed by ISO | Developed for TCP/IP networking |
| More detailed | More commonly used in real networks |
| Has separate Presentation and Session layers | These are included in Application layer |

---

# 17. Switching

Switching is a technique used to transfer data from a source device to a destination device through a network.

The main types of switching are:

1. Circuit Switching
2. Packet Switching
3. Message Switching

---

# 18. Circuit Switching

In circuit switching, a dedicated communication path is established between the sender and receiver before communication begins.

### Example

Traditional telephone networks.

### Advantages

- Dedicated path
- Constant bandwidth
- Predictable communication

### Disadvantages

- Wastes resources when the connection is idle
- Connection setup is required
- Not efficient for bursty data

---

# 19. Packet Switching

In packet switching, data is divided into small units called **packets**.

Each packet may travel through the network to reach the destination.

### Example

The Internet mainly uses packet switching.

### Advantages

- Efficient use of network resources
- Suitable for Internet communication
- Multiple users can share network resources

### Disadvantages

- Packets may be delayed
- Packets may arrive out of order
- Network congestion can occur

---

# 20. Message Switching

In message switching, the complete message is stored at an intermediate device before being forwarded to the next device.

This method is also called **store-and-forward switching**.

### Advantages

- No dedicated path is required
- Efficient use of network resources

### Disadvantages

- Requires large storage
- Can cause significant delay

---

# 21. Circuit vs Packet vs Message Switching

| Feature | Circuit Switching | Packet Switching | Message Switching |
|---|---|---|---|
| Path | Dedicated | Shared | Shared |
| Data | Continuous stream | Packets | Complete message |
| Delay | Low after setup | Variable | Usually high |
| Storage | Less | Some buffering | Large storage required |
| Example | Telephone network | Internet | Store-and-forward systems |

---

# Quick Revision

## OSI Model

**7 Layers:**

Application  
↓  
Presentation  
↓  
Session  
↓  
Transport  
↓  
Network  
↓  
Data Link  
↓  
Physical

## TCP/IP Model

**4 Layers:**

Application  
↓  
Transport  
↓  
Internet  
↓  
Network Access

## Switching

- Circuit Switching → Dedicated path
- Packet Switching → Data divided into packets
- Message Switching → Complete message stored and forwarded

---

# Learning Goals

After studying this topic, I should be able to:

- Explain the concept of layering
- Describe all 7 OSI layers
- Explain the TCP/IP model
- Compare OSI and TCP/IP
- Explain circuit switching
- Explain packet switching
- Explain message switching
- Compare different switching techniques
