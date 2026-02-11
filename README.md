

# MidRiver Health – Incident Response Investigation

This repository documents a simulated enterprise incident response investigation
involving unauthorized VPN access, privilege escalation, malware execution,
and confirmed data exfiltration.

---

## Incident Overview

An alert was triggered following anomalous VPN authentication activity
associated with workstation FIN-WS-077 in the Finance VLAN.

Subsequent analysis revealed:

- Unauthorized VPN login from 203.0.113.45
- Immediate privilege escalation (Event ID 4672 – SeRestorePrivilege)
- Execution of updater.exe from Temp directory
- Encoded PowerShell activity
- Sustained outbound HTTPS data transfers exceeding 2GB
- Windows audit logs cleared prior to disconnect

---

## Investigation Phases

1. Initial Alert & VPN Log Review
2. Host-Based Log Correlation
3. Privilege Escalation Analysis
4. Malware Execution & Command Activity
5. Network & DNS Correlation
6. NetFlow Exfiltration Analysis
7. Containment & Defensive Recommendations

---

## Skills Demonstrated

- Multi-source log correlation (VPN, Windows, DNS, Firewall, NetFlow, IDS)
- Timeline reconstruction
- Privilege escalation detection
- Encoded PowerShell analysis
- Data exfiltration pattern identification
- Anti-forensics detection (log clearing)
- Incident containment strategy development

---

📄 Full Investigation Report:  
[View Report](./MidRiver-Health-Incident-Response.pdf)

---

## Tools & Technologies

- Windows Security Event Logs
- VPN Authentication Logs
- DNS Resolver Logs
- Firewall Egress Logs
- NetFlow Analysis
- IDS Alerts
- Wireshark (validation)
- Splunk (log correlation)
