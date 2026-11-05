<div align="center">

# 🦈 NETWORKWALKS-B084-WK1-PM1-CYBERSECURITY-PMx-WIRESHARK-EXTRA
### Walk through Wireshark labs to investigate network activity logs

[![Skill](https://img.shields.io/badge/Skill-Cybersecurity-red?style=for-the-badge&logo=shield&logoColor=white)](https://github.com)
[![Ver](https://img.shields.io/badge/Ver-Virtualbox_v7.2-blue?style=for-the-badge&logo=virtualbox&logoColor=white)](https://github.com)
[![Kali Linux](https://img.shields.io/badge/Kali_Linux-v2026.3-orange?style=for-the-badge&logo=kalilinux&logoColor=white)](https://github.com)
[![Skill](https://img.shields.io/badge/Skill-Linux-darkgrey?style=for-the-badge&logo=linux&logoColor=white)](https://github.com)
[![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-teal?style=for-the-badge&logo=cisco&logoColor=white)](https://github.com)
[![Penetration Testing](https://img.shields.io/badge/Penetration_Testing-Lab-black?style=for-the-badge&logo=letsencrypt&logoColor=white)](https://github.com)
[![Skill](https://img.shields.io/badge/Skill-Virtualization-red?style=for-the-badge&logo=vmware&logoColor=white)](https://github.com)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com)
[![NetworkWalks](https://img.shields.io/badge/NetworkWalks-orange?style=for-the-badge&logo=network-wired&logoColor=white)](https://github.com)
[![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-Practice-darkred?style=for-the-badge&logo=hackthebox&logoColor=white)](https://github.com)

---

</div>

## 🧪 Lab Investigations Breakdown

### 🔬 Lab 3: HTTP Traffic Analysis & Credential Extraction
* **Objective:** Detect unencrypted plaintext credentials transmitted across the network.
* **Key Tasks:** Applied the `http.request.method == "POST"` filter to isolate login events and parsed the HTML form URL-encoded data payload to recover credentials.

### 🕵️‍♂️ Lab 4: Detecting Malicious Port Scans
* **Objective:** Identify reconnaissance activity targeting internal network infrastructure.
* **Key Tasks:** Analyzed high-frequency TCP SYN packets without subsequent connections (`tcp.flags.syn == 1 and tcp.flags.ack == 0`) originating from a single host.

### 🔍 Lab 5: DNS Tunneling Detection
* **Objective:** Discover covert data exfiltration masquerading as standard domain name lookups.
* **Key Tasks:** Filtered for unusual traffic volumes using `dns` and investigated high counts of anomalous, long-string TXT and AAAA query records.

### 📦 Lab 4: Automated Malware Beaconing Activity
* **Objective:** Track down compromised sandbox assets communicating with external Command and Control (C2) servers.
* **Key Tasks:** Analyzed recurring, exact-interval HTT
