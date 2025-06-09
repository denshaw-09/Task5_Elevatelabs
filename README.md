# Network Traffic Analysis Report

## Overview
This project analyzes network traffic using **Wireshark** by capturing packets across different protocols. 
The study focuses on **DNS, TCP, and HTTP (port 80)** to examine communication patterns, request-response interactions, and potential performance insights.

## Tools Used
- **Windsurf** (Packet Capture & Analysis)
- **Command Line (eg., ping example.com)** for generating ICMP traffic
- **Filtering by Protocols:** DNS, TCP, HTTP

## Captured Protocols

### **1. DNS (Domain Name System)**

- Resolves domain names to IP addresses.
- Queried domains included:
  - `ssl.gstatic.com`
  - `googleusercontent.com`
- Successful queries confirmed proper name resolution.

### **2. TCP (Transmission Control Protocol)**
- Ensured reliable communication via **SYN, SYN-ACK, ACK** handshake.
- Data exchange confirmed between local and remote servers.
- Some retransmissions observed, indicating possible network congestion.

### **3. HTTP (Port 80)**
- Represents unencrypted web traffic.
- Displays request-response behavior between the client and web servers.
- HTTP traffic suggests websites using **non-secure HTTP connections** instead of HTTPS.

## Packet Capture Summary
- **File Format:** `.pcap` (Packet Capture)
- **Captured via:** Windsurf filtering and manual analysis
- **Exported Packets:** DNS, TCP, HTTP

## Key Findings
✅ **Network connectivity confirmed** via successful packet exchanges.  
✅ **Latency Insights**—TCP timestamps provide round-trip time measurements.  
✅ **Potential Packet Loss Detected**—Retransmissions indicate network delays or dropped packets.  
⚠️ **Unencrypted HTTP Traffic Noted**—HTTP connections over port 80 lack security encryption.  

## Conclusion
This analysis successfully identifies **domain resolution, TCP-based communication, and HTTP browsing behavior**. 

## How to Use the `.pcap` File
1. Open the `.pcap` file in **Wireshark** or Windsurf.
2. Apply **protocol filters** (DNS, TCP, HTTP) to review captured packets.
3. Analyze request-response interactions and network performance metrics.

---

### **Next Steps**
- **Analyze additional encrypted HTTPS (port 443) traffic.**
- **Examine deeper packet structures for retransmission causes.**
- **Assess potential security risks in unencrypted traffic.**

---
