# Splunk SIEM Lab: Sysmon + Log Forwarding + Detection Use Cases

## Overview
Built a SIEM lab to collect and forward system logs from Windows and Linux endpoints into Splunk for centralized monitoring and analysis.  
Implemented Sysmon on Windows to generate detailed telemetry and created dashboards + searches for three detection use cases. :contentReference[oaicite:1]{index=1}

## Environment (Lab)
- SIEM: Splunk Web (lab)
- Windows endpoints: Windows Event Logs + Sysmon telemetry :contentReference[oaicite:2]{index=2}
- Linux endpoint: /var/log via Splunk Universal Forwarder :contentReference[oaicite:3]{index=3}

## What I Implemented
### Log Collection
- Installed and validated Sysmon on Windows systems :contentReference[oaicite:4]{index=4}
- Forwarded Windows Event Logs and Sysmon logs to Splunk :contentReference[oaicite:5]{index=5}
- Forwarded Linux /var/log to Splunk using Universal Forwarder :contentReference[oaicite:6]{index=6}

### Detection Use Cases
1. **Admin user creation detection** (new user created with administrative privileges) :contentReference[oaicite:7]{index=7}
2. **Failed logon detection** (Windows Event ID **4625**) :contentReference[oaicite:8]{index=8}
3. **Linux log activity monitoring** (/var/log ingestion monitoring) :contentReference[oaicite:9]{index=9}

## Repo Structure
- `searches/` → SPL queries for each use case
- `setup/` → setup notes for Sysmon and forwarders
- `screenshots/` → dashboard evidence

## Next Improvements
- Add CIM / InfoSec App normalization & correlation (planned) :contentReference[oaicite:10]{index=10}
- Add alert actions (email/webhook) and tuning notes

## Disclaimer
All testing was performed in an isolated lab environment for educational and defensive security purposes only.
