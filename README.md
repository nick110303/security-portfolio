# Security Portfolio

A collection of offensive and defensive security projects, including a full-scope
simulated penetration test, malware analysis writeups, and SIEM-based detection
engineering work.

## 🔴 Penetration Testing

**[Enterprise Network Penetration Test](./pentesting/pentest-report)**

A simulated full-scope penetration test of a fictional enterprise network,
covering Active Directory exploitation, web application testing, and
post-exploitation.

- **Scope:** Windows & Linux systems, Active Directory, web applications
- **Findings:** 13 total — 6 Critical, 5 High, 2 Medium (SQL injection, LFI, RCE,
  broken access control, AD misconfigurations)
- **Tools:** Nmap, Burp Suite, Metasploit, Hydra, Impacket, ffuf

➡️ [View report](./pentesting/pentest-report)

## 🟣 Malware Analysis

**[Raccoon Info-Stealer Analysis](./malware-analysis/malware-report)**

Static and dynamic analysis of a Raccoon-family information stealer distributed
as "wotsuper 2.1," including unpacking a Delphi/BobSoft-packed binary, tracing
credential and cookie theft across multiple browsers, and identifying C2
communication via DNS.

- **Key findings:** Packed executable (BobSoft Mini Delphi), .cab-based payload
  extraction, anti-VM checks via keyboard/locale APIs, credential & cookie theft,
  IP exfiltration via IPLogger, C2 domains identified via DNS/reverse DNS
- **Tools:** PEStudio, x32dbg + Scylla, Process Monitor, Process Explorer,
  Regshot, Wireshark, FakeDNS, YARA

➡️ [View analysis](./malware-analysis/malware-report)

## About Me

Hi, I'm Nicholas Gionti. I'm an aspiring SOC analyst with a strong interest in
detection engineering, log analysis, and blue team operations. My malware
analysis work reflects that focus directly, and my pentest experience gives me
insight into attacker behavior that I bring into building better detections.

**Connect:** [LinkedIn](https://www.linkedin.com/in/nicholas-gionti/) • [Resume](#)
