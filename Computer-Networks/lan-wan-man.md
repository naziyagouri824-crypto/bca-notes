# LAN, WAN, MAN, Topologies & LAN Access Techniques

## 1. Types of Computer Networks

Computer networks can be classified according to their geographical coverage.

The three important types are:

1. LAN
2. MAN
3. WAN

---

# 2. LAN

LAN stands for **Local Area Network**.

A LAN connects computers and devices within a small geographical area such as:

* Home
* Office
* School
* College
* Computer laboratory

### Features of LAN

* Covers a small area
* High data transfer speed
* Usually privately owned
* Easy to manage
* Relatively low cost

### Example

A computer lab where all computers are connected to the same network.

---

# 3. MAN

MAN stands for **Metropolitan Area Network**.

It covers a larger geographical area than LAN, usually a city or metropolitan area.

### Features of MAN

* Covers a city or large campus
* Larger than LAN
* Smaller than WAN
* Can connect multiple LANs

### Example

A network connecting different branches of an organization within the same city.

---

# 4. WAN

WAN stands for **Wide Area Network**.

It covers a very large geographical area such as countries or continents.

### Features of WAN

* Covers large geographical areas
* Connects multiple LANs and MANs
* Uses communication links over long distances
* More complex than LAN
* Usually has higher communication costs

### Example

The Internet is the largest example of a WAN.

---

# 5. LAN vs MAN vs WAN

| Feature   | LAN                | MAN                       | WAN                                   |
| --------- | ------------------ | ------------------------- | ------------------------------------- |
| Full Form | Local Area Network | Metropolitan Area Network | Wide Area Network                     |
| Area      | Small              | City/Metropolitan area    | Very large area                       |
| Speed     | High               | Medium to high            | Generally lower than LAN              |
| Ownership | Usually private    | Private or public         | Often uses multiple service providers |
| Example   | College lab        | City-wide network         | Internet                              |

---

# 6. Network Topology

Network topology refers to the physical or logical arrangement of devices and connections in a network.

Important LAN topologies are:

1. Star Topology
2. Bus Topology
3. Ring Topology

---

# 7. Star Topology

In Star Topology, all devices are connected to a central device such as a switch or hub.

### Structure

```text
          Computer
              |
              |
Computer — Switch — Computer
              |
              |
          Computer
```

### Advantages

* Easy to install
* Easy to manage
* Failure of one cable usually affects only one device
* Easy to add or remove devices
* Easy troubleshooting

### Disadvantages

* Failure of the central device can affect the entire network
* Requires more cable
* Installation cost can be higher

### Example

Modern office and school networks commonly use star topology.

---

# 8. Bus Topology

In Bus Topology, all devices are connected to a single main cable called the **backbone**.

### Structure

```text
Computer     Computer     Computer
    |            |            |
================================
           Main Cable
```

### Advantages

* Simple design
* Requires less cable
* Low installation cost for small networks

### Disadvantages

* Failure of the main cable can affect the entire network
* Difficult to troubleshoot
* Performance decreases when more devices are added
* Limited scalability

---

# 9. Ring Topology

In Ring Topology, each device is connected to two other devices, forming a closed loop.

### Structure

```text
Computer ─── Computer
    |             |
    |             |
Computer ─── Computer
```

### Advantages

* Data can travel in an organized manner
* Equal access to network resources
* No central device is required

### Disadvantages

* Failure of one connection can affect communication
* Adding or removing devices can be difficult
* Troubleshooting can be harder

---

# 10. Star vs Bus vs Ring

| Feature          | Star     | Bus          | Ring                |
| ---------------- | -------- | ------------ | ------------------- |
| Central Device   | Required | Not required | Not required        |
| Main Cable       | No       | Yes          | No                  |
| Failure Handling | Easy     | Difficult    | Can affect the ring |
| Installation     | Easy     | Simple       | Moderate            |
| Troubleshooting  | Easy     | Difficult    | Difficult           |
| Scalability      | Good     | Limited      | Limited             |

---

# 11. LAN Access Techniques

LAN access techniques are methods used to control how multiple devices share a common communication medium.

Important access techniques are:

* ALOHA
* CSMA/CD
* CSMA/CA
* Token Ring
* Token Bus

---

# 12. ALOHA

ALOHA is a random access protocol used to control access to a shared communication channel.

A device can transmit data whenever it has data to send.

If two devices transmit at the same time, a **collision** may occur.

After a collision, the devices wait for a random amount of time and retransmit.

### Types of ALOHA

1. Pure ALOHA
2. Slotted ALOHA

---

## Pure ALOHA

In Pure ALOHA, a device can transmit at any time.

### Working

1. Device sends data.
2. If transmission is successful, communication continues.
3. If a collision occurs, the device waits for a random time.
4. The device retransmits the data.

### Disadvantage

The probability of collision is relatively high.

---

## Slotted ALOHA

In Slotted ALOHA, time is divided into fixed slots.

A device can start transmission only at the beginning of a time slot.

This reduces the possibility of collisions compared with Pure ALOHA.

---

# 13. CSMA

CSMA stands for **Carrier Sense Multiple Access**.

Before transmitting data, a device listens to the communication channel.

If the channel is free, the device can transmit.

If the channel is busy, the device waits.

---

# 14. CSMA/CD

CSMA/CD stands for **Carrier Sense Multiple Access with Collision Detection**.

It is designed to detect collisions during data transmission.

### Working

1. Device listens to the channel.
2. If the channel is free, it starts transmission.
3. The device continues to monitor the channel.
4. If a collision is detected, transmission stops.
5. The device waits for a random period.
6. The device retransmits the data.

### Important Point

CSMA/CD was traditionally associated with **shared half-duplex Ethernet**.

---

# 15. CSMA/CA

CSMA/CA stands for **Carrier Sense Multiple Access with Collision Avoidance**.

It tries to avoid collisions before they occur.

It is mainly associated with **wireless networks such as Wi-Fi**.

### Working

1. Device checks whether the channel is free.
2. If the channel is busy, it waits.
3. If the channel is free, it waits for the required period.
4. Device selects a random backoff time.
5. Device transmits when the backoff period ends.
6. An acknowledgement may be used to confirm successful reception.

### Important Point

Wireless devices cannot reliably detect collisions in the same way as traditional shared Ethernet, so collision avoidance is used.

---

# 16. CSMA/CD vs CSMA/CA

| Feature            | CSMA/CD                                                | CSMA/CA                                                |
| ------------------ | ------------------------------------------------------ | ------------------------------------------------------ |
| Full Form          | Carrier Sense Multiple Access with Collision Detection | Carrier Sense Multiple Access with Collision Avoidance |
| Main Idea          | Detect collision                                       | Try to avoid collision                                 |
| Common Use         | Traditional shared Ethernet                            | Wireless LAN/Wi-Fi                                     |
| Collision Handling | Collision is detected after it occurs                  | Attempts to reduce collision probability               |

---

# 17. Token Ring

Token Ring is a controlled access technique in which a special frame called a **token** circulates around the network.

Only the device holding the token can transmit data.

### Working

1. Token circulates through the network.
2. Device receives the token.
3. Device sends data.
4. After transmission, the token is released.
5. Token moves to the next device.

### Advantages

* Prevents collisions
* Provides organized access
* Predictable waiting time

### Disadvantages

* Token management is required
* Failure of network components can affect communication
* Less common in modern networks

---

# 18. Token Bus

Token Bus is a controlled access technique in which devices form a logical ring over a physical bus network.

A token is passed between devices in a predefined logical order.

Only the device holding the token can transmit.

### Advantages

* Prevents collisions
* Provides controlled access
* Predictable communication

### Disadvantages

* Token management is required
* Failure can affect communication
* More complex than random access methods

---

# 19. Network Reliability

Network reliability refers to the ability of a network to continue functioning correctly and provide communication services.

### Issues Affecting Network Reliability

* Hardware failure
* Cable failure
* Network congestion
* Power failure
* Software problems
* Configuration errors
* Server failure
* Natural disasters

### Methods to Improve Reliability

* Use backup devices
* Use redundant network paths
* Regularly maintain hardware
* Use backup power
* Monitor network performance
* Keep systems updated
* Use reliable network equipment

---

# 20. Network Security

Network security means protecting network devices, data, and communication from unauthorized access and attacks.

### Common Security Issues

* Unauthorized access
* Malware
* Viruses
* Phishing
* Data theft
* Password attacks
* Denial-of-Service attacks
* Eavesdropping

### Methods to Improve Network Security

* Use strong passwords
* Use firewalls
* Use encryption
* Keep software updated
* Use antivirus/anti-malware software
* Apply access controls
* Monitor network activity
* Take regular backups

---

# 21. Quick Revision

## Network Types

**LAN** → Small area

**MAN** → City/metropolitan area

**WAN** → Large geographical area

## Topologies

**Star** → Central device

**Bus** → Single backbone cable

**Ring** → Closed loop

## Access Techniques

**ALOHA** → Random access

**CSMA/CD** → Detects collisions

**CSMA/CA** → Tries to avoid collisions

**Token Ring** → Token circulates in a logical ring

**Token Bus** → Token passes in logical order over a bus

## Reliability

Focuses on keeping the network available and functioning correctly.

## Security

Focuses on protecting the network and data from unauthorized access and attacks.

---

# Learning Goals

After studying this topic, I should be able to:

* Explain LAN, MAN, and WAN
* Compare LAN, MAN, and WAN
* Explain Star, Bus, and Ring topologies
* Compare different LAN topologies
* Explain ALOHA
* Explain CSMA/CD
* Explain CSMA/CA
* Explain Token Ring
* Explain Token Bus
* Understand network reliability issues
* Understand basic network security issues

