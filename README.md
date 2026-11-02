# Security Portfolio

A collection of defensive and offensive security projects, including SOC alert
investigations, malware analysis writeups, and a full-scope simulated penetration
test.

## 🔵 SOC Case Reports

Alert investigations from the TryHackMe SOC Simulator, written up as case reports
in a consistent format: summary, evidence, timeline, IOCs, assessment, and actions
taken. Each one covers how the alert was triaged, what the logs and threat intel
showed, and why it was closed or escalated.

- **Focus:** Alert triage, log analysis, threat intel lookups, and incident documentation
- **Tools:** Splunk, TryDetectThis, TryHackMe SOC Simulator

| Alert | Type | Verdict | Report |
|---|---|---|---|
| 8815 | Phishing (Amazon impersonation) | True Positive | [View report](./soc-case-reports/SOC-Simulator-Phishing-Alert-8815.pdf) |

*New investigations are added as I complete them.*

## 🟣 Malware Analysis

**[Raccoon Info-Stealer Analysis](./malware-analysis/malware-report.pdf)**

Static and dynamic analysis of a Raccoon-family information stealer distributed
as "wotsuper 2.1," including unpacking a Delphi/BobSoft-packed binary, tracing
credential and cookie theft across multiple browsers, and identifying C2
communication via DNS.

- **Findings:** Packed executable (BobSoft Mini Delphi), .cab-based payload
  extraction, anti-VM checks via keyboard/locale APIs, credential & cookie theft,
  IP exfiltration via IPLogger, C2 domains identified via DNS/reverse DNS
- **Tools:** PEStudio, x32dbg + Scylla, Process Monitor, Process Explorer,
  Regshot, Wireshark, FakeDNS, YARA

➡️ [View analysis](./malware-analysis/malware-report.pdf)

## 🔴 Penetration Testing

**[Enterprise Network Penetration Test](./pentesting/pentest-report.pdf)**

A simulated full-scope penetration test of a fictional enterprise network,
covering Active Directory exploitation, web application testing, and
post-exploitation.

- **Scope:** Windows & Linux systems, Active Directory, web applications
- **Findings:** 13 total - 6 Critical, 5 High, 2 Medium (SQL injection, LFI, RCE,
  broken access control, AD misconfigurations)
- **Tools:** Nmap, Burp Suite, Metasploit, Hydra, Impacket, ffuf

➡️ [View report](./pentesting/pentest-report.pdf)

## About Me

Hi, I'm Nicholas Gionti. I'm an aspiring SOC analyst with a strong interest in
detection engineering, log analysis, and blue team operations. I hold CompTIA
Security+ and Network+, completed the TryHackMe SOC Level 1 path, and rank in
the top 3% on the platform. My SOC case work and malware analysis reflect that
blue team focus directly, and my pentest experience gives me insight into
attacker behavior that I bring into building better detections.

**Connect:** [LinkedIn](https://www.linkedin.com/in/nicholas-gionti/)
