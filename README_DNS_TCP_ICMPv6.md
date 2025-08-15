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
   - **Screenshot:**
     ![Wireshark Installation](images/install.png)

2. **Started Packet Capture**
   - Opened Wireshark and selected the active network interface (Wi-Fi).
   - Clicked the **Start Capture** button (blue shark fin).
   - **Screenshot:**
     ![Interface Selection](images/interface.png)

3. **Generated Network Traffic**
   - Opened a web browser and visited multiple websites.
   - Used the `ping` command to test connectivity to `8.8.8.8`.
   - **Screenshot:**
     ![Ping Command](images/ping.png)

4. **Stopped Capture**
   - Stopped capture after ~1 minute using the red square button.
   - **Screenshot:**
     ![Capture Stop](images/stop.png)

5. **Filtered Packets by Protocol**
   - Applied filters:
     - `dns` → To view domain name resolution requests.
     - `tcp` → To view TCP connections.
     - `icmpv6` → To view ICMPv6 (Internet Control Message Protocol for IPv6) packets.
   - **Screenshot:**
     ![Protocol Filter](images/filter.png)

6. **Identified Protocols**
   - Observed the following protocols in the capture:
     - **DNS** – Domain name queries and responses.
     - **TCP** – Transport layer communication.
     - **ICMPv6** – Control messages used in IPv6 networking.

7. **Exported Capture**
   - Saved capture as `network_capture.pcap` for further study.
   - **Screenshot:**
     ![Export PCAP](images/export.png)

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

## 📂 Output Files
- **network_capture.pcap** – Exported packet capture file.

---

## 📜 Conclusion
Using Wireshark, I successfully captured live network traffic, identified **DNS**, **TCP**, and **ICMPv6** protocols, and analyzed their packet details. This exercise demonstrated how different protocols operate within the network stack, including both IPv4 and IPv6 traffic analysis.

---

✅ **Note:**
Replace the image paths like `images/install.png` with your actual screenshot filenames when you upload them to your repository.
