# Networking Basics 0

Welcome to **Networking Basics 0**, a project designed to introduce you to the fundamentals of computer networking. The goal is for you to be able to explain core network concepts without relying on Google.

---

## Table of Contents

1. [Resources](#resources)
2. [Learning Objectives](#learning-objectives)
3. [Requirements](#requirements)
4. [More Info](#more-info)
5. [Tasks](#tasks)
   - [0. OSI model](#0-osi-model)
   - [1. Types of network](#1-types-of-network)
   - [2. MAC and IP address](#2-mac-and-ip-address)
   - [3. UDP and TCP](#3-udp-and-tcp)
   - [4. TCP and UDP ports](#4-tcp-and-udp-ports)
   - [5. Is the host on the network](#5-is-the-host-on-the-network)

---

## Resources

Read or watch:

- [OSI model](https://en.wikipedia.org/wiki/OSI_model)
- [Different types of network](https://en.wikipedia.org/wiki/Computer_network#Types_of_network)
- [LAN network](https://en.wikipedia.org/wiki/Local_area_network)
- [WAN network](https://en.wikipedia.org/wiki/Wide_area_network)
- [Internet](https://en.wikipedia.org/wiki/Internet)
- [MAC address](https://en.wikipedia.org/wiki/MAC_address)
- [What is an IP address](https://en.wikipedia.org/wiki/IP_address)
- [Private and public address](https://en.wikipedia.org/wiki/IP_address#Private_addresses)
- [IPv4 and IPv6](https://en.wikipedia.org/wiki/IPv6)
- [Localhost](https://en.wikipedia.org/wiki/Localhost)
- [TCP and UDP](https://en.wikipedia.org/wiki/Transmission_Control_Protocol)
- [TCP/UDP ports List](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)
- [What is ping /ICMP](https://en.wikipedia.org/wiki/Ping_(networking_utility))
- [Positional parameters](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_02.html)

**man or help**:

- `netstat`
- `ping`

---

## Learning Objectives

By the end of this project, you should be able to **explain to anyone**, **without the help of Google**:

### OSI Model
- What it is  
- How many layers it has  
- How it is organized  

### LAN
- Typical usage  
- Typical geographical size  

### WAN
- Typical usage  
- Typical geographical size  

### Internet
- What it is  

### IP Address
- What are the 2 types of IP address  
- What is `localhost`  
- What is a subnet  
- Why IPv6 was created  

### TCP/UDP
- What are the 2 mainly used data transfer protocols for IP (transfer level on the OSI schema)  
- What is the main difference between TCP and UDP  

### Port
- What is a port  
- Memorize **SSH (22)**, **HTTP (80)**, and **HTTPS (443)** port numbers  

### Tool/Protocol for Checking Network Connectivity
- What tool/protocol is often used to check if a device is connected to a network

---

## Requirements

### General

- **Allowed editors**: `vi`, `vim`, `emacs`
- All your Bash script files will be interpreted on **Ubuntu 20.04 LTS**
- All your files should end with a **new line**
- A `README.md` file, at the root of the folder of the project, is **mandatory**
- All your Bash script files **must be executable**
- Your Bash script must pass `shellcheck` **without any error**
- The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all your Bash scripts should be a comment explaining what the script is doing

---