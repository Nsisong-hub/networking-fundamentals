# networking-fundamentals

## OSI Model Overview
The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes network communication in seven layers:

1. **Physical Layer**: Handles physical connections and transmission of raw data.
   - *Example*: Ethernet cables, fiber optics, Wi-Fi signals.

2. **Data Link Layer**: Manages node-to-node communication and error detection.
   - *Example*: MAC addresses in Ethernet frames.

3. **Network Layer**: Determines packet routing across networks.
   - *Example*: IP addressing and routing.

4. **Transport Layer**: Ensures reliable data transmission using protocols like TCP and UDP.
   - *Example*: TCP guarantees delivery of an email.

5. **Session Layer**: Maintains and manages communication sessions.
   - *Example*: Logging into a website and keeping the session active.

6. **Presentation Layer**: Translates, encrypts, and compresses data.
   - *Example*: SSL/TLS encryption for secure web browsing.

7. **Application Layer**: Interfaces with end-user applications.
   - *Example*: Web browsers using HTTP/HTTPS, email clients using SMTP.

---

## Subnetting Calculation
Given an IP range of **192.168.1.0/24**, we have divided it into four subnets using a subnet calculator:

| Subnet | Network Address | First Usable IP | Last Usable IP | Broadcast Address |
|--------|----------------|----------------|----------------|-------------------|
| 1      | 192.168.1.0/26 | 192.168.1.1    | 192.168.1.62   | 192.168.1.63     |
| 2      | 192.168.1.64/26 | 192.168.1.65   | 192.168.1.126  | 192.168.1.127    |
| 3      | 192.168.1.128/26 | 192.168.1.129  | 192.168.1.190  | 192.168.1.191    |
| 4      | 192.168.1.192/26 | 192.168.1.193  | 192.168.1.254  | 192.168.1.255    |

### Screenshots
Subnetting calculator screenshots are available in the `subnetting_screenshots/` folder.

---

## TCP/IP Protocol Suite in Action
When a user loads a webpage (e.g., `www.example.com`), the TCP/IP model processes data through four layers:

1. **Application Layer** (HTTP/HTTPS) sends a request to the web server.
2. **Transport Layer** (TCP) segments the data and ensures reliability with acknowledgments.
3. **Internet Layer** (IP) determines the best route for data packets.
4. **Network Access Layer** (Ethernet/Wi-Fi) transmits data over the physical network.

Upon reaching the destination, the reverse process reconstructs the webpage for the user.

---

## Repository Structure
```
networking-fundamentals/
│── README.md  # Summary of OSI, subnetting, and TCP/IP
│── networking_fundamentals.md  # Detailed report
│── subnetting_screenshots/  # Folder containing subnet calculator screenshots
```

This repository serves as documentation for networking concepts, including the OSI model, subnetting, and TCP/IP communication.
