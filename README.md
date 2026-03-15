# 🌐 NetPractice: The Networking Blueprint

A technical guide to mastering Layer 3 networking, subnetting, and routing. This repository contains the logic and strategies needed to navigate the challenges of the 42 NetPractice project.

<p align="center">
    <img src="https://img.shields.io/badge/42-School-blue" alt="42 School Badge">
    <img src="https://img.shields.io/badge/Status-Completed-brightgreen" alt="Status Badge">
</p>

<p align="center">
  <img src="Imags/Into.png" alt="NetPractice Banner">
</p>

## 🏙️ **The "Digital City" Analogy**

To understand networking, stop thinking about numbers and start thinking about architecture:

* **IP Address:** Your house address in the city.

* **Subnet Mask:** The "Zoning Law" that decides how big your neighborhood is.

* **Router:** The "Traffic Cop" 🚦 standing at the intersection of two neighborhoods.

* **Switch:** The "Community Hall" where everyone inside the same neighborhood meets.

* **Default Gateway:** The "Main Exit" out of your neighborhood to the rest of the world.

## 🛠️ Core Concepts Simplified

### **1. Subnetting: Slicing the Pizza** 🍕

A large network is like a giant pizza. Subnetting is how we slice it so different teams (web servers, databases, users) don't get in each other's way.

```
graph LR
    A[Internet] --> B((Router))
    subgraph Neighborhood_A [Subnet 1: Public Web]
    B --> C[Web Server]
    end
    subgraph Neighborhood_B [Subnet 2: Private DB]
    B --> D[Database]
    end
    style Neighborhood_A fill:#f9f,stroke:#333
    style Neighborhood_B fill:#bbf,stroke:#333
```

### **2. The TCP/IP Handshake: The Formal Intro**

Before data moves, computers perform a "**Three-Way Handshake.**" It’s like a polite phone call:

**SYN:** "Hey, can you hear me?"

**SYN-ACK:** "Yes! I can hear you, can you hear me?"

**ACK:** "Perfect, let's talk."