<div align="center">

# 🦈 NetworkWalks-B084-WK1-PM1
## Cybersecurity PMx · Wireshark Extra

### 🔍 Walk through Wireshark labs to investigate network activity logs

<br>

![Wireshark](https://img.shields.io/badge/Wireshark-Packet%20Analysis-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-PMx-0A2540?style=for-the-badge&logo=hackthebox&logoColor=white)
![Ethical Hacking](https://img.shields.io/badge/Ethical-Hacking-2ea44f?style=for-the-badge&logo=kalilinux&logoColor=white)

![Network Traffic Analysis](https://img.shields.io/badge/Skill-Network%20Traffic%20Analysis-blue?style=flat-square&logo=wireshark&logoColor=white)
![Network Basics](https://img.shields.io/badge/Skill-Network%20Basics-orange?style=flat-square&logo=cisco&logoColor=white)
![Protocol Analysis](https://img.shields.io/badge/Skill-Protocol%20Analysis-purple?style=flat-square&logo=gnometerminal&logoColor=white)
![NetworkWalks](https://img.shields.io/badge/Series-NetworkWalks-red?style=flat-square&logo=github&logoColor=white)

</div>

---

## 📖 About

Hands-on walkthroughs for investigating network activity logs with **Wireshark**. Each lab follows a real-world analyst workflow: capture, filter, inspect, and conclude.

## 🎯 What You'll Practice

| | Skill | Focus |
|---|-------|-------|
| 🌐 | **Network Basics** | Layers, addressing, common ports |
| 📡 | **Protocol Analysis** | TCP, UDP, DNS, HTTP, ICMP, ARP |
| 🕵️ | **Network Traffic Analysis** | Spotting suspicious flows and anomalies |
| 🧪 | **Ethical Hacking** | Understanding attacker behaviour from the defender's side |

## 🧰 Tools

- 🦈 Wireshark
- 💾 Sample `.pcap` / `.pcapng` capture files
- 🐧 Linux or Windows workstation

## 🚀 Getting Started

1. 📥 Clone this repository
2. 🦈 Open the capture files in Wireshark
3. 📝 Follow each lab walkthrough in order
4. ✅ Check your findings against the notes

## 🔎 Handy Display Filters

```text
ip.addr == 192.168.1.10      # traffic to or from a host
tcp.port == 443              # filter by port
dns                          # DNS queries and responses
http.request                 # HTTP requests only
tcp.flags.syn == 1 && tcp.flags.ack == 0   # SYN scan candidates
```

## ⚠️ Disclaimer

For **educational use only**. Analyse only traffic you own or are authorised to inspect.

---

<div align="center">

Made with 💙 for network defenders · Happy hunting 🦈

</div>
