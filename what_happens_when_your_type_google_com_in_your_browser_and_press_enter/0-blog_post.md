![Header Image](https://github.com/sifir-gun/holbertonschool-network/blob/main/what_happens_when_your_type_google_com_in_your_browser_and_press_enter/google_networking.png)

# What happens when you type https://www.google.com into your browser?

**Guney Tasdelen 🧑🏻‍💻**  
Web Application Developer | Python | HTML | CSS | Next.js | SQL | C Machine Learning & Deep Learning 🧠

*16 janvier 2025*

*Note: This article is written as part of a pedagogical exercise aimed at explaining in detail the flow of a request when entering a URL in a browser and pressing Enter. Enjoy reading!*

## 1. Introduction

The question "What happens when you type https://www.google.com into your browser and press Enter?" is a classic in technical interviews for Software Engineer, DevOps/SRE, or Front-End positions. It evaluates your understanding of the web stack and the mechanisms that operate "under the hood."

As future engineers or developers, it is essential to master fundamental concepts such as DNS, TCP/IP, network security, and server communication. Moreover, having an in-depth knowledge of these steps strengthens your ability to diagnose and solve performance or security issues.

In this article, we will break down step by step what happens from the moment you press Enter to the moment the page displays in your browser.

![Distributed Web Infrastructure - Architecture Diagram](https://github.com/sifir-gun/holbertonschool-network/blob/main/what_happens_when_your_type_google_com_in_your_browser_and_press_enter/Architecture_Diagram.png)

## 2. Step by Step

### 2.1 DNS Request

DNS (Domain Name System) is often the first step in the process. When you type https://www.google.com, your browser must resolve the domain name www.google.com into an IP address (e.g., 142.250.185.36).

- The browser first checks its local DNS cache to see if it already has a match
- If not found, it queries the DNS resolver (often your Internet Service Provider's DNS or a public DNS service such as Google DNS)
- If needed, the resolver queries the root and domain DNS servers until it finds the IP address associated with the domain

This conversion of "domain name ↔ IP address" is crucial: machines truly only understand IP addresses. DNS therefore acts like the phone book of the internet.

### 2.2 TCP/IP

Once the IP address is obtained, your computer establishes a TCP (Transmission Control Protocol) connection over the IP (Internet Protocol) layer. TCP/IP is the suite of protocols that manage the routing of data packets between devices connected to the internet.

- TCP guarantees reliable and orderly delivery of packets
- IP handles routing from point A (your machine) to point B (Google's server)

During TCP negotiation, we talk about the 3-way handshake:

1. SYN (client → server)
2. SYN-ACK (server → client)
3. ACK (client → server)

### 2.3 Firewall

Before reaching Google's servers, the request may pass through several firewalls. Firewalls are installed to protect a network or a machine from malicious or unauthorized traffic.

- Your computer may have a local firewall
- Your company/university may have a network firewall
- Google also protects its infrastructure using firewalls and other filtering systems (such as intrusion detection systems)

If a firewall deems your request suspicious (an unauthorized port, unusual traffic, etc.), the connection can be blocked.

### 2.4 HTTPS/SSL

When you see https://, it means communication is encrypted through TLS/SSL (Transport Layer Security / Secure Sockets Layer).

SSL/TLS Handshake: Your browser and the server negotiate a method of encryption and exchange certificates to ensure the server is who it claims to be (authentication).
Once the secure connection is established, all data is exchanged in encrypted form to prevent interception and content manipulation (Man-in-the-Middle attacks).

### 2.5 Load-Balancer

Google has a large number of servers all over the world. To distribute the load (and connect you to the closest or least busy data center), Google uses a load balancer.

- The load balancer receives the request
- It decides which server to send it to (based on location, CPU load, etc.)

This step ensures better responsiveness and high availability: if one server fails, the load balancer redirects traffic to other servers.

### 2.6 Web Server

Once the request has arrived at the web server (e.g., Nginx, Apache, or Google's internal Web Server), that server handles the following:

- Analyzes the HTTP(S) request
- Checks whether it has the static or dynamic content requested (such as HTML pages, images, style sheets, scripts)
- Transfers the request to an Application Server if more complex processing is needed

### 2.7 Application Server

In many systems, the web server then communicates with an application server (e.g., Node.js, Python Flask, Java Spring Boot, etc.). This server can handle business logic, run scripts, query a database, etc.

- It receives request data (session, cookies, URL parameters, etc.)
- It performs the required logic, for example validating a user ID, processing a form, or generating dynamic content

### 2.8 Database

If the application needs data, it connects to a database (SQL or NoSQL).

- For instance, Google can consult a vast database indexing the world's web pages
- The application server executes a query (SELECT, INSERT, etc.), retrieves the response, and then formats it to send back to the web server

Once the response is fully constructed, it returns in the reverse path: database → application server → web server → load balancer → your browser.

## 3. Conclusion: The Display in the Browser

Finally, your browser receives the HTTP response, containing the HTML code, CSS styles, JavaScript, etc. It then proceeds to:

1. Parse the code
2. Build the DOM (Document Object Model)
3. Download external resources (images, style sheets, scripts)
4. Execute the JavaScript and display the page

And there you have it! What seems like a simple press of the Enter key actually triggers a complex series of operations involving multiple machines across the globe.

![Sequence diagram illustrating the steps of loading a web page](https://github.com/sifir-gun/holbertonschool-network/blob/main/what_happens_when_your_type_google_com_in_your_browser_and_press_enter/Sequence_Diagram.png)

## 5. Sources

- MDN Web Docs – DNS
- Google Cloud Load Balancing
- How HTTPS Works
- SearchNetworking TechTarget: TCP/IP Definition

*Thank you for reading this article! You now know what really happens when you type a URL and press Enter. This in-depth understanding will be very useful for your projects and future technical interviews. Feel free to share your thoughts in the comments or on social media. Happy exploring the web!*
