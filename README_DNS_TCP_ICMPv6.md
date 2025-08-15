# Wireshark Packet Capture & Analysis

## 📌 Objective
To capture and analyze network traffic using **Wireshark**, identify different protocols in use (DNS, TCP, and ICMPv6), and summarize the findings in a `.pcap` file for further analysis.

---

## 🛠 Tools Used
- **Wireshark** – Network packet analyzer
- **Operating System** – Windows / Linux / macOS
- **Browser / Ping utility** – To generate network traffic

---

## 📋 Steps Performed

1. **Installed Wireshark**
   - Downloaded from [wireshark.org](https://www.wireshark.org/) and installed.

2. **Started Packet Capture**
   - Opened Wireshark and selected the active network interface (Wi-Fi).
   - Clicked the **Start Capture** button (blue shark fin).
   - 
3. **Generated Network Traffic**
   - Opened a web browser and visited multiple websites.
   - Used the `ping` command to test connectivity to `8.8.8.8`.

4. **Stopped Capture**
   - Stopped capture after ~1 minute using the red square button.

5. **Filtered Packets by Protocol**
   - Applied filters:
     - `dns` → To view domain name resolution requests.
     - `tcp` → To view TCP connections.
     - `icmpv6` → To view ICMPv6 (Internet Control Message Protocol for IPv6) packets.

6. **Identified Protocols**
   - Observed the following protocols in the capture:
     - **DNS** – Domain name queries and responses.
     - **TCP** – Transport layer communication.
     - **ICMPv6** – Control messages used in IPv6 networking.

7. **Exported Capture**
   - Saved capture as `dns.pcap` `icmpv6.pcap` `tcp.pcap` for further study.

8. **Summarized Findings**
   - **DNS**: Queries for domain names and their IP resolutions.
   - **TCP**: Connection establishment (SYN, ACK) and data transfer.
   - **ICMPv6**: Used for diagnostics (e.g., ping) and network discovery in IPv6.

---

## 📊 Sample Findings Table

| Protocol | No. of Packets | Description |
|----------|---------------|-------------|
| DNS      | 30            | Domain name lookups |
| TCP      | 200           | Transport layer communication |
| ICMPv6   | 15            | IPv6 control messages and diagnostics |

---


## 📜 Conclusion
Using Wireshark, I successfully captured live network traffic, identified **DNS**, **TCP**, and **ICMPv6** protocols, and analyzed their packet details. This exercise demonstrated how different protocols operate within the network stack, including both IPv4 and IPv6 traffic analysis.

---

