# Networking Basics 1

Welcome to **Networking Basics 1**, a project designed to deepen your understanding of networking concepts, especially around localhost, IP addresses, and port listening. By the end of this project, you should be able to explain the following, **without the help of Google**:

---

## Table of Contents

1. [Resources](#resources)
2. [Learning Objectives](#learning-objectives)
3. [Requirements](#requirements)
4. [Tasks](#tasks)
   - [0. Change your home IP](#0-change-your-home-ip)
   - [1. Show attached IPs](#1-show-attached-ips)
   - [2. Port listening on localhost](#2-port-listening-on-localhost)
5. [Author](#author)

---

## Resources

**Read or watch**:

- [What is localhost](https://en.wikipedia.org/wiki/Localhost)
- [What is 0.0.0.0](https://en.wikipedia.org/wiki/0.0.0.0)
- [What is the hosts file](https://en.wikipedia.org/wiki/Hosts_(file))
- [Netcat examples](https://www.geeksforgeeks.org/netcat-nc-command-usage-examples/)

**man or help**:

- `ifconfig`
- `telnet`
- `nc`
- `cut`

---

## Learning Objectives

At the end of this project, you are expected to be able to **explain to anyone**, **without the help of Google**:

1. **General**
   - What is `localhost/127.0.0.1`  
   - What is `0.0.0.0`  
   - What is `/etc/hosts`  
   - How to display your machine’s active network interfaces  

---

## Requirements

- **Allowed editors**: `vi`, `vim`, `emacs`
- All your files will be interpreted on **Ubuntu 20.04 LTS**
- All your files should end with a **new line**
- A `README.md` file, at the root of the folder of the project, is **mandatory**
- All your Bash scripts must be **executable**
- Your Bash scripts must pass **Shellcheck** (version `0.7.0` via `apt-get`) without any errors
- The first line of all your Bash scripts should be exactly:
  #!/usr/bin/env bash
