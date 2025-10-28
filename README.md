# Task-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark
Perform a live packet capture in Wireshark and analyze it to identify key network protocols and traffic patterns.

# Capture and Analyze Network Traffic Using Wireshark

#Objective
Capture live network packets using *Wireshark* and identify basic protocols and traffic types.

---

## Tools Used
- *Wireshark* (Network Packet Analyzer)
- *Kali Linux* (or Windows)

---

## ⚙ Steps Performed

1. *Installed Wireshark*
   ```bash
   sudo apt update
   sudo apt install wireshark -y
   sudo usermod -aG wireshark $USER

   Selected the active network interface eth0

   Clicked the blue Start Capture button
Generated traffic by visiting websites and running:
ping google.com -c 4
Stopped the capture after 1 minute.

Filtered and Analyzed Protocols

Used filters:
http → to see web traffic
dns → to see domain lookups
tcp → to see transport layer packets
icmp → to view ping traffic

Findings:
DNS packets showed hostname resolution queries.
HTTP packets captured browsing activity and website requests.
ICMP packets confirmed connectivity using echo requests and replies.
All packets were successfully recorded and analyzed in Wireshark.
