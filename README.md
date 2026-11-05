<div align="center">

# 🦈 NetworkWalks-B084-WK1-PM1
## Cybersecurity PMx · Wireshark SOC Labs

### 🔍 Walk through Wireshark labs to investigate network activity logs

<br>

![Wireshark](https://img.shields.io/badge/Wireshark-Packet%20Analysis-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-PMx-0A2540?style=for-the-badge&logo=hackthebox&logoColor=white)
![Score](https://img.shields.io/badge/Labs%203--8-100%25-2ea44f?style=for-the-badge&logo=checkmarx&logoColor=white)

![Network Traffic Analysis](https://img.shields.io/badge/Skill-Network%20Traffic%20Analysis-blue?style=flat-square&logo=wireshark&logoColor=white)
![Network Basics](https://img.shields.io/badge/Skill-Network%20Basics-orange?style=flat-square&logo=cisco&logoColor=white)
![Protocol Analysis](https://img.shields.io/badge/Skill-Protocol%20Analysis-purple?style=flat-square&logo=gnometerminal&logoColor=white)
![NetworkWalks](https://img.shields.io/badge/Series-NetworkWalks-red?style=flat-square&logo=github&logoColor=white)

</div>

---

## 🏆 Results at a Glance

| # | Lab | Focus | Completed | Score |
|:-:|-----|-------|:---------:|:-----:|
| 3 | 🎯 Identify the Attacker's IP | SYN port scan detection | 1 Nov 2026 | ✅ 100 / 100 |
| 4 | 💬 Follow TCP Stream | Reconstructing a chat session | 5 Nov 2026 | ✅ 100 / 100 |
| 5 | 📄 Follow TCP Stream, part 2 | Pages, files and downloads | 5 Nov 2026 | ✅ 100 / 100 |
| 6 | 🔓 HTTP Plain Text Credentials | Credentials sent in the clear | 28 Oct 2026 | ✅ 100 / 100 |
| 7 | 🔨 Brute Force Catch | Spotting repeated failed logins | 28 Oct 2026 | ✅ 100 / 100 |
| 8 | 📞 VoIP Call Replay | Call setup and voice stream analysis | 29 Oct 2026 | ✅ 100 / 100 |

> 🌟 **Perfect scores across all six labs.** Every task was marked *Correct*.

---

## 🧪 Lab Investigations Breakdown

### 🎯 Lab 3: Identify the Attacker's IP

> **Objective:** Find who is scanning the network, and what they are after.

- 📥 Capture the traffic
- 🔎 Show only SYN packets
- 🕵️ Find the attacker and the target
- 🔌 Identify the source port and the ports probed
- 🟢 Tell open ports apart from closed ports, using the reply for closed ports
- 🏷️ Name the attack type

### 💬 Lab 4: Follow TCP Stream

> **Objective:** Reassemble a conversation from split packets into readable text.

- 📥 Capture the traffic
- 🔌 Find the chat port and who started the chat
- 🔢 Note the stream number and the size of the chat
- 🆘 Work out who needs help, and which drive has the problem
- 🔑 Pull out the temporary password and the guest Wi-Fi password
- 🎨 Find the text colour used

### 📄 Lab 5: Follow TCP Stream, Part 2

> **Objective:** Trace web pages and file transfers hidden inside a stream.

- 📥 Capture the traffic
- 🌐 Find the pages and where the content is hidden
- 🔢 Find the right stream
- 🗝️ Recover the code word and the backup server
- ↔️ Determine the direction of traffic and the status code
- 📦 Identify the downloaded file and who made the report

### 🔓 Lab 6: HTTP Plain Text Credentials

> **Objective:** Show why unencrypted HTTP logins are a risk.

- 📥 Capture the traffic
- 📡 Identify the protocol and the method used
- 🔐 Find the login page and the PC that signed in
- 🔁 Count the login attempts
- 👤 Extract the username and the password from the packet details line
- 🛠️ Recommend the fix

### 🔨 Lab 7: Brute Force Catch

> **Objective:** Detect a password-guessing attack and find the point of compromise.

- 📥 Capture the traffic
- 📡 Identify the protocol, the target and the attacker
- 👤 Find the username under attack
- ❌ Read the failure code and count the failed logins
- ✅ Find the success code and the password that worked
- 🏷️ Name the attack type

### 📞 Lab 8: VoIP Call Replay

> **Objective:** Decode a phone call and see what a capture can expose.

- 📥 Capture the traffic
- ☎️ Identify the call setup protocol and the voice protocol
- 🧑 Find the caller extension and caller name
- 🎧 Identify the codec and who answered
- 💳 Recover the card number and expiry date spoken on the call
- 🛠️ Recommend the fix

---

## 🔎 Handy Display Filters

```text
tcp.flags.syn == 1 && tcp.flags.ack == 0   # SYN packets (scan detection)
tcp.stream eq 0                            # isolate one TCP conversation
http.request.method == "POST"              # form submissions and logins
sip                                        # call signalling
rtp                                        # voice media streams
```

## 💡 Key Takeaways

- 🔍 A flood of SYN packets from one source across many ports is a classic scan signature.
- 💬 **Follow TCP Stream** turns fragmented packets into a readable transcript.
- 🔓 Plain HTTP and unencrypted VoIP expose credentials and sensitive data to anyone on the wire.
- 🛡️ The fix is encryption (HTTPS, TLS, SRTP) and strong authentication controls.

## ⚠️ Disclaimer

For **educational use only**. Analyse only traffic you own or are authorised to inspect.

<div align="center">

Made with 💙 for network defenders · Happy hunting 🦈

</div>
