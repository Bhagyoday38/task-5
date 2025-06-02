# task-5
# 🕵️ Network Traffic Capture and Analysis Using Wireshark

## 📌 Objective

Capture live network packets using Wireshark on Kali Linux and analyze them to identify basic network protocols and traffic types.

---

## 🛠️ Tools Used

- **Wireshark** – Network protocol analyzer
- **Kali Linux** – Operating system for penetration testing and security auditing
- **Terminal / Browser** – To generate sample network traffic

---

## 🚀 Steps Performed

### 1. Install Wireshark (if not pre-installed)
```bash
sudo apt update
sudo apt install wireshark -y
2. Identify Active Network Interface
bash

ip a
3. Start Wireshark
bash

sudo wireshark
Selected the active network interface for capturing packets.

4. Generate Network Traffic
Pinging Google:

bash

ping google.com
Browsing to https://example.com using Firefox

5. Stop Packet Capture
After approximately 1 minute of activity, the capture was stopped using the stop button in Wireshark.

6. Filter and Analyze Packets
Applied the following filters to isolate traffic:

dns

http

icmp

tcp

7. Export the Capture
Saved the capture as network_traffic.pcap using:
File > Save As > .pcap format

🔎 Protocols Identified
Protocol	Description	Port	Example
DNS	Domain resolution protocol	UDP 53	Query for google.com
HTTP	Web traffic protocol	TCP 80	GET request to example.com
ICMP	Ping/echo requests	N/A	Echo request/reply to 8.8.8.8

📈 Observations
DNS queries resolved domain names before initiating HTTP traffic.

HTTP traffic showed client-server GET requests.

ICMP traffic from ping showed request-reply sequence.

TCP three-way handshakes observed before data transfer.

✅ Outcome
Gained hands-on experience in capturing and analyzing network traffic.

Learned to identify and filter common protocols in packet captures.

Developed basic protocol awareness using Wireshark


