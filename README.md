# 🕵️ Insider Threat Case Study – Suspicious Data Access

## 📘 Project Overview
This project simulates an insider threat investigation based on anomalous access behaviors within a defense contracting environment. It demonstrates investigative analysis, behavioral pattern detection, and threat reporting as practiced in real-world DFIR and threat hunting workflows.

## 🎯 Objective
Analyze user activity logs to determine whether suspicious access to classified files by a cleared employee constitutes a malicious insider threat.

## 🗂️ Data Sources
- Simulated file access logs
- VPN session records
- Endpoint behavior patterns
- User activity timeline
- Threat intel (MITRE ATT&CK)

## 🧠 Investigative Process
- Correlated access timestamps with sensitive file paths
- Mapped user behavior to known MITRE ATT&CK techniques
- Compared outbound connections to threat intel sources
- Reviewed prior HR/disciplinary issues tied to user

## 🔍 Key Findings
- Repeated access to `/classified/intel/2023_ops` outside working hours
- Unusual VPN access from foreign IP (192.168.x.x) between 0200-0300 PST
- Traffic aligned with ATT&CK T1041 (Exfiltration over C2 channel)
- User history includes previous policy violations

## ✅ Conclusion
Subject exhibited multiple red flags consistent with potential insider threat behavior. Further digital forensics, such as drive imaging and HR escalation, are recommended.

## 🛡️ Recommendations
- Revoke Subject X’s credentials and escalate to HR/Security
- Perform forensic acquisition of Subject X’s endpoint
- Implement alerting on off-hours file access to sensitive folders

## 🛠️ Tools Used
- Python (log parsing)
- Excel (timeline correlation)
- MITRE ATT&CK Navigator
- draw.io (timeline visualization)

