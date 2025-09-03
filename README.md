# Hoplight
AI-assisted Security Operations Platform prototype with real-time SOC, analytics, investigation, detection/response, governance, and reporting, with privacy-by-design and PII redaction.

**Hoplight** is a prototype security operations platform I designed and built to explore how **AI-powered analytics** can enhance SOC workflows.  
It integrates traditional SIEM functions with AI-driven correlation, investigation, and reporting — all with **privacy-by-design controls** like PII redaction before AI processing.  

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
![Status: Prototype](https://img.shields.io/badge/status-prototype-blue)
![Stack: Node.js • MongoDB • Wazuh](https://img.shields.io/badge/stack-Node.js%20•%20MongoDB%20•%20Wazuh-informational)

---

## Key Features

### Real-Time SOC Suite
- Group-level security overview (endpoints, signals, alerts)  
- AI-driven **threat clustering** and correlation  
- **Risk escalation engine** tracking repeat and evolving threats  

### Advanced Analytics Suite
- In-depth threat analytics with historical context  
- Endpoint **behavioral baselines** per group  
- **Pattern engine** to detect deviations from expected activity  

### Investigation Suite
- **Forensic analysis workflows** using AI + correlation  
- **MITRE ATT&CK chain reconstruction** and kill chain mapping  
- **Threat intelligence**: IOC matching, campaign linkage  

### Detection & Response Suite
- **Correlation engine** for multi-source signals  
- **Enhanced AI triage** to reduce false positives  
- Incident response metrics: MTTR, SLA compliance, analyst logs  

### Governance & Compliance Suite
- Custom dashboards for **PCI DSS, HIPAA, GDPR, or client frameworks**  
- AI-generated **executive summaries** (daily/weekly/monthly) with graphs & KPIs  
- Technical report exports for SOCs and MSP analysts  

### Audit & Baselines
- Per-group baseline definitions and deviation tracking  
- Full audit logs for compliance and forensic readiness  

---

## Security & Privacy
- **Privacy by design**: PII scrubbed before AI sees data  
- **TLS-encrypted traffic**, **SSH keys-only**, secrets managed via `.env`  
- **MongoDB hardening**: role-based access, SCRAM-SHA-256 auth, TLS in transit  
- Audit logging for all privileged actions  

---

## 📸 Screenshots
---
<p align="center">
  <img src="Threat Monitoring Tab.png" width="900" alt="Threat Monitoring – real-time clustering and IOC overview">
</p>
---
- **Enterprise Threat Intelligence:** IOC matches, campaign activity, actor profiles  
  <img src="Threat Intelligence Tab.png" width="900" alt="Threat Intelligence Center">

- **Attack Chain Reconstruction:** MITRE ATT&CK mapping, kill-chain analysis, narrative generation  
  <img src="Attack Chain Reconstruction Tab.png" width="900" alt="Attack Chain Reconstruction">

- **Dynamic Correlation Engine:** accuracy/threshold metrics and analysis actions  
  <img src="Dynamic Correlation Tab.png" width="900" alt="Dynamic Correlation Engine">

- **Baseline Management:** per-group baselines, deviations, accuracy  
  <img src="Baseline Management Tab.png" width="900" alt="Baseline Management">

---

## Architecture Overview
**Stack:**  
- Backend: **Node.js & Wazuh** (129 APIs across 13 modules)  
- Database: **MongoDB** (schemas + baselines + audit logs)  
- Frontend: **JavaScript** dashboard (work in progress)  
- AI Integration: PII redaction → AI analysis → reporting pipeline  

**Deployment:**  
- Hosted on hardened VPS (Ubuntu)  
- TLS, SSH keys-only, firewall rules (80/443 only)  

---

## Current Status
✅ Backend complete and operational  
🟡 Frontend dashboards and executive reporting in progress  

---

## Roadmap
- [ ] Finalize executive reporting UI  
- [ ] Expand AI correlation for bulk signal analysis  
- [ ] Improve dependency management and module linkage  
- [ ] Publish sample demo data for portfolio/demo purposes  

---

## Disclaimer
Hoplight is a **prototype / personal project**.  
It is not deployed in production environments and is shared here for **portfolio and educational purposes only**.
