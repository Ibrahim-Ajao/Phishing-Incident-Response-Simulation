# 🛡️ Phishing Incident Response Simulation

This project simulates a real-world phishing email investigation process, modeled on how a SOC analyst would triage, investigate, and report a phishing attack.

---

## 📌 Project Goals

- Analyze a simulated phishing email
- Identify and extract IOCs (URLs, IPs, domains)
- Use public tools (VirusTotal, URLScan.io, WHOIS)
- Document the investigation with a formal incident report

---

## 🧰 Tools Used

| Tool        | Purpose                             |
|-------------|-------------------------------------|
| Email Header Analyzer | Understand mail routing, spoofing |
| VirusTotal  | Detect malicious URLs/files         |
| URLScan.io  | Simulate site behavior              |
| WHOIS/IPInfo | Reveal domain & hosting details     |

---

## 📨 Email Sample (Used in This Simulation)

**Sender**: PayPal <security@paypalsecure-email.com>  
**Subject**: Unusual Login Attempt Detected  
**Link**: `https://secure-paypal-update.com/login`  
**Body**: See `email_sample.txt` for full content.

---

## 🔍 Analysis Steps

- Header parsed via [Google MessageHeader Tool](https://toolbox.googleapps.com/apps/messageheader/)
- URL scanned via VirusTotal & URLScan.io
- Domain WHOIS and IP address info extracted and verified
- IOCs extracted and listed in `/analysis/ioc_scan_results.md`
- All steps and findings summarized in the final report

---

## 📄 Files Overview

| File/Folder       | Description                             |
|-------------------|-----------------------------------------|
| `email_sample.txt`| The phishing email text (simulated)     |
| `/analysis/`      | Raw findings from online scans          |
| `/report/`        | Final incident response report          |
| `/screenshots/`   | Screenshots from tools used             |

---

## 🔗 Sample IOCs (Indicators of Compromise)

- `secure-paypal-update.com`
- Domain IP: `203.0.113.44`
- Created: July 20, 2025
- Flags: Phishing, typo domain, Whois privacy

---

## 📄 Final Report Location

`/report/phishing_incident_report.md`  
Includes: timeline, IOCs, tools used, and recommendations for next steps.

---

## 🎓 Learning Outcomes

- Email header triage & spoofing detection
- URL and file threat intelligence using open-source tools
- IOC extraction and correlation
- Writing a clear, structured incident response report

---

## 👤 Author

**Ajao Ibrahim Adewale**  
SOC Analyst Trainee | Google Cybersecurity Professional Certificate Graduate  
📧 your.email@example.com  
🔗 [GitHub Portfolio](https://github.com/yourusername)

---
