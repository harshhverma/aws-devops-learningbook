# Networking Fundamentals for DevOps

## Environment
- Networking Basics
- DevOps Networking
- Cloud Networking
- AWS Networking Concepts

---

# What is Networking?

Networking is the process of connecting devices so they can communicate and exchange data with each other.

Networking is one of the core foundations of:
- DevOps
- Cloud Computing
- System Administration
- Kubernetes
- Distributed Systems

---

# What is an IP Address?

An IP Address is a unique identifier assigned to a device on a network.

Example:
```text
192.168.1.10
```

IPv4 consists of:
- 4 bytes
- 32 bits total
- Each segment ranges from 0–255

---

# Why IP Address is Used

IP addresses are used to:
- identify devices
- establish communication
- send and receive data across networks

Without IP addresses, devices cannot communicate over a network.

---

# Types of IP Addresses

## Public IP
- Accessible over internet
- Used for public communication

Example:
```text
EC2 Public IP
```

---

## Private IP
- Used inside private networks
- Not directly accessible from internet

Example:
```text
AWS Private Subnet Instances
```

---

# What is a Subnet?

A subnet is a smaller network created from a larger network.

Subnetting helps improve:
- security
- organization
- network isolation
- resource management

---

# Public vs Private Subnet

## Public Subnet
- Has internet access
- Used for web servers, bastion hosts

---

## Private Subnet
- No direct internet access
- Used for databases and internal services

---

# What is CIDR?

CIDR stands for:
```text
Classless Inter-Domain Routing
```

CIDR notation defines:
- network size
- number of available IP addresses

Example:
```text
192.168.1.0/24
```

---

# CIDR Formula

```text
32 - CIDR = Host Bits
```

Example:
```text
/24
```

Host bits:
```text
32 - 24 = 8
```

Available IPs:
```text
2^8 = 256 IPs
```

Usable Hosts:
```text
254
```

---

# Common CIDR Ranges

| CIDR | Total IPs | Usable Hosts |
|---|---|---|
| /24 | 256 | 254 |
| /25 | 128 | 126 |
| /26 | 64 | 62 |
| /27 | 32 | 30 |
| /28 | 16 | 14 |

---

# Network and Host Portion

Every IP address contains:
- Network Portion
- Host Portion

## Network Portion
Identifies the network.

## Host Portion
Identifies the device inside the network.

Example:
```text
192.168.1.10/24
```

Network:
```text
192.168.1
```

Host:
```text
10
```

---

# What is a Port?

Ports are unique numbers assigned to applications running on a system.

Ports help incoming traffic reach the correct application.

---

# Common Ports

| Service | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| MySQL | 3306 |
| Jenkins | 8080 |

---

# Why Ports are Important

Ports allow multiple services to run on the same machine without conflicts.

Example:
- SSH on Port 22
- Website on Port 80
- Jenkins on Port 8080

Same server, different services.

---

# Networking in AWS

AWS networking concepts include:
- VPC
- Public Subnet
- Private Subnet
- Internet Gateway
- Route Tables
- Security Groups

---

# DevOps Relevance

Networking is important in DevOps because it is used in:
- Cloud infrastructure
- Kubernetes networking
- Load balancing
- CI/CD systems
- Server communication
- Security configuration

---

# Interview Questions & Answers

## What is an IP Address?

An IP Address is a unique identifier assigned to a device on a network for communication.

---

## Difference Between Public and Private IP

| Public IP | Private IP |
|---|---|
| Accessible from internet | Internal network use only |
| Globally unique | Used within private networks |

---

## What is Subnetting?

Subnetting is the process of dividing a large network into smaller logical networks to improve security and network management.

---

## What is CIDR?

CIDR is a notation used to define network size and available IP addresses within a subnet.

---

## What is the Difference Between Network and Host Portion?

The network portion identifies the network, while the host portion identifies the specific device inside that network.

---

## What is a Port?

A port is a logical communication endpoint used to identify specific applications or services running on a system.

---

## Why are Ports Important?

Ports help route incoming traffic to the correct application running on a server.

---

## Why is Networking Important in DevOps?

Networking is important in DevOps because cloud infrastructure, servers, containers, APIs, and deployment systems communicate over networks.

---

# Key Takeaways

- Learned networking fundamentals
- Understood IP addressing
- Learned subnetting concepts
- Understood CIDR ranges
- Learned network vs host portion
- Understood ports and communication
- Connected networking concepts with DevOps and AWS
