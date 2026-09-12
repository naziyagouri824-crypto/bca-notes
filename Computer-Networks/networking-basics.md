# 🌐 Computer Networks — Networking Basics

A **computer network** is a group of interconnected computers and devices that communicate with each other and share data and resources.

## 📌 Why Do We Need Computer Networks?

Computer networks are used for:

* Sharing files and data
* Sharing hardware resources
* Communication
* Internet access
* Resource sharing
* Centralized management

## 📡 Transmission Media

**Transmission media** is the path through which data travels from one device to another.

Transmission media can be divided into:

1. Guided Media
2. Unguided Media

### Guided Media

In guided media, signals travel through a physical path such as a cable.

Examples:

* Twisted Pair Cable
* Coaxial Cable
* Optical Fiber

### Unguided Media

In unguided media, signals travel through air or space without a physical cable.

Examples:

* Radio waves
* Microwaves
* Infrared

---

# 🔌 Twisted Pair Cable

Twisted pair cable consists of pairs of insulated copper wires twisted together.

The twisting helps reduce electromagnetic interference and crosstalk.

### Types

* UTP — Unshielded Twisted Pair
* STP — Shielded Twisted Pair

### Advantages

* Low cost
* Easy to install
* Easy to maintain
* Commonly used in LANs

### Disadvantages

* Limited distance
* More affected by interference than optical fiber

### Uses

* Telephone networks
* Ethernet networks
* Local Area Networks

---

# 📺 Coaxial Cable

Coaxial cable contains a central copper conductor surrounded by insulation, a metallic shield, and an outer protective covering.

### Advantages

* Better protection against interference than twisted pair
* Higher bandwidth than basic twisted pair
* Durable

### Disadvantages

* More expensive than twisted pair
* Less flexible
* Installation can be more difficult

### Uses

* Cable television
* Broadband connections
* Communication systems

---

# 💡 Optical Fiber

Optical fiber is a transmission medium that uses **light signals** to transmit data through thin strands of glass or plastic.

### Main Parts

* Core
* Cladding
* Protective coating

### Advantages

* Very high bandwidth
* High transmission speed
* Low signal loss
* Immune to electromagnetic interference
* Suitable for long distances

### Disadvantages

* More expensive
* Installation requires specialized equipment
* More delicate than copper cables

### Uses

* Internet backbone
* Long-distance communication
* Fiber-to-the-home connections
* High-speed networks

---

# 🔀 Hub

A **hub** is a networking device that connects multiple devices in a network.

When a hub receives data, it broadcasts the data to all connected devices.

```text id="3v2f8x"
        Hub
     /   |   \
    PC   PC   PC
```

### Key Point

A hub does not intelligently determine the destination device.

---

# 🌉 Bridge

A **bridge** connects and filters traffic between network segments.

It uses **MAC addresses** to determine whether data should be forwarded between segments.

### Key Point

A bridge can reduce unnecessary traffic between network segments.

---

# 🔀 Switch

A **switch** connects devices within a network and forwards data to the appropriate destination port using MAC addresses.

```text id="p3qk3r"
        Switch
      /   |   \
     PC   PC   PC
```

### Advantages

* Efficient data forwarding
* Reduces unnecessary traffic
* Better performance than a hub
* Commonly used in LANs

---

# 🌐 Router

A **router** connects different networks and forwards packets between them.

Routers use **IP addresses** to determine the appropriate path for packets.

```text id="x7f8u2m"
LAN ─── Router ─── Internet
```

### Functions

* Connects different networks
* Forwards packets
* Selects routes
* Connects local networks to the Internet

---

# 📊 Hub vs Switch vs Router

| Device | Main Function                        | Address Used              |
| ------ | ------------------------------------ | ------------------------- |
| Hub    | Broadcasts data to connected devices | No intelligent addressing |
| Switch | Forwards data within a LAN           | MAC address               |
| Router | Connects different networks          | IP address                |

## 🧠 Quick Revision

```text id="9zj2kf"
Twisted Pair → Copper wires twisted together

Coaxial Cable → Central conductor + shielding

Optical Fiber → Uses light for data transmission

Hub → Broadcasts data

Bridge → Connects/filters network segments

Switch → Forwards frames using MAC addresses

Router → Connects networks and forwards packets using IP addresses
```

## 🎯 Learning Goals

* Understand computer networks
* Understand transmission media
* Learn twisted pair cable
* Learn coaxial cable
* Understand optical fiber
* Understand hubs and bridges
* Understand switches
* Understand routers
* Compare common networking devices

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
