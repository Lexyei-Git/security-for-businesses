# NIST Cybersecurity Framework for SMBs

The **NIST Cybersecurity Framework (CSF) 2.0** is a high‑level, voluntary framework created by the US National Institute of Standards and Technology (NIST) to help organizations manage and reduce cybersecurity risk.

This document explains NIST CSF 2.0 in plain language for small and medium businesses (SMBs) and shows how the controls in this repository map to the framework’s six Functions.

---

## 1. What NIST CSF 2.0 is (plain language)

NIST CSF 2.0 is:

- A **flexible, high‑level structure** with **six core Functions** that cover the cybersecurity lifecycle.  
- Designed to be **scalable** – SMBs can use it without needing enterprise‑level resources.  
- A **common language** for communicating cybersecurity priorities to management, customers and partners.

The six Functions (NIST CSF 2.0) are:

1. **Govern** – Establish and oversee the cybersecurity strategy and program.  
2. **Identify** – Understand your assets, risks and vulnerabilities.  
3. **Protect** – Implement safeguards to limit or contain the impact of potential cybersecurity events.  
4. **Detect** – Identify cybersecurity events in a timely manner.  
5. **Respond** – Take action regarding a detected cybersecurity incident.  
6. **Recover** – Restore capabilities or services impaired due to a cybersecurity incident.

**SMB takeaway**: You do not need to implement everything at once. Start with a **Current Profile** (what you do now) and build toward a **Target Profile** (what you want to achieve) over 12–24 months.

---

## 2. NIST CSF 2.0 Functions explained for SMBs

Each Function has **Categories** and **Subcategories**. This guide focuses on **practical SMB actions** and maps them to your repository content.

### 2.1 Govern (GV)
**Purpose**: Establish and oversee the cybersecurity strategy and program.

**SMB actions**:
- Define basic **roles and responsibilities** for security (for example, who is the security lead, who approves policies).  
- Create simple **policies** (acceptable use, passwords/MFA, incident reporting) using `policies/`.  
- Review security **metrics and progress** quarterly with leadership (for example, MFA coverage, patching status, awareness training completed).  
- Use `5-maturity-roadmaps/` to create a **12‑month security plan** aligned with business goals.

**Repository mapping**:
- `policies/README.md` – Policy governance for SMBs.  
- `5-maturity-roadmaps/12-month-plan.md` – Practical roadmap planning.

### 2.2 Identify (ID)
**Purpose**: Understand your assets, risks and vulnerabilities.

**SMB actions**:
- Create a **simple asset inventory** using `templates/asset-inventory.csv` and `2-where-to-start/simple-asset-inventory.md`.  
- Perform a **basic risk assessment** using `templates/basic-risk-assessment.csv` and `2-where-to-start/basic-risk-assessment.md`.  
- Maintain a **vendor inventory** using `templates/vendor-inventory-and-assessment.csv`.

**Repository mapping**:
- `2-where-to-start/simple-asset-inventory.md` and `basic-risk-assessment.md`.  
- `3-practical-controls/vendor-and-third-party-risk-basics.md`.

### 2.3 Protect (PR)
**Purpose**: Implement safeguards to limit or contain the impact of potential cybersecurity events.

**SMB actions**:
- Enable **MFA** and strong passwords (`passwords-and-mfa.md`).  
- Implement **patching and secure configuration** (`patching-and-updates.md`, `device-hardening-and-configuration.md`).  
- Deploy **antivirus/endpoint protection** (`antivirus-and-anti-malware.md`).  
- Set up **backups** (`backups.md`).  
- Train staff on **phishing and awareness** (`email-and-phishing.md`, `security-awareness-and-training.md`).

**Repository mapping**:
- Most of `3-practical-controls/` (access control, patching, backups, antivirus, awareness, cloud/SaaS security, Wi‑Fi/VPN, physical security).

### 2.4 Detect (DE)
**Purpose**: Identify cybersecurity events in a timely manner.

**SMB actions**:
- Enable **logging and monitoring** on key systems (`logging-and-monitoring-basics.md`).  
- Review security alerts from email protection, antivirus, cloud platforms and network tools.  
- Encourage staff to **report suspicious activity** early (`incident-reporting-policy.md`).

**Repository mapping**:
- `logging-and-monitoring-basics.md`.  
- `incident-reporting-policy.md`.

### 2.5 Respond (RS)
**Purpose**: Take action regarding a detected cybersecurity incident.

**SMB actions**:
- Follow your **simple incident response playbook** (`incident-response-basics.md`).  
- Use `templates/incident-log.csv` to document incidents and track follow‑up actions.  
- Notify management, legal/privacy contacts and external parties as required.

**Repository mapping**:
- `incident-response-basics.md`.  
- `templates/incident-log.csv`.

### 2.6 Recover (RC)
**Purpose**: Restore capabilities or services impaired due to a cybersecurity incident.

**SMB actions**:
- **Restore from clean backups** (`backups.md`).  
- Test recovery procedures periodically.  
- Communicate recovery status to leadership and affected stakeholders.  
- Update processes based on lessons learned from incidents.

**Repository mapping**:
- `backups.md`.  
- `incident-response-basics.md` (recovery phase).

---

## 3. How your repository maps to NIST CSF 2.0

This table shows the main repository content mapped to NIST CSF Functions:

| NIST CSF Function | Repository Content |
|-------------------|--------------------|
| **Govern (GV)** | `policies/README.md`, `5-maturity-roadmaps/` |
| **Identify (ID)** | `2-where-to-start/simple-asset-inventory.md`, `basic-risk-assessment.md`, `3-practical-controls/vendor-and-third-party-risk-basics.md` |
| **Protect (PR)** | Most of `3-practical-controls/` (MFA, patching, backups, antivirus, awareness, access control, hardening, cloud security) |
| **Detect (DE)** | `logging-and-monitoring-basics.md`, `incident-reporting-policy.md` |
| **Respond (RS)** | `incident-response-basics.md`, `templates/incident-log.csv` |
| **Recover (RC)** | `backups.md`, `incident-response-basics.md` (recovery steps) |

This mapping helps you:
- **Communicate progress** to management (“We are strong on Protect, working on Detect”).  
- **Identify gaps** (“We have no Detect capability yet”).  
- **Plan improvements** using the roadmap files.

---

## 4. NIST CSF 2.0 for SMBs: practical roadmap

NIST provides a **Small Business Quick‑Start Guide** that aligns with this repository:

**Phase 1: Kick‑start (0–3 months)**
- Asset inventory and basic risk assessment (`2-where-to-start/`).  
- Enable MFA, backups, patching and antivirus (`3-practical-controls/`).

**Phase 2: Foundation (3–12 months)**
- Policies, logging, vendor risk management, incident response (`policies/`, `incident-response-basics.md`).  
- Regular awareness training.

**Phase 3: Continuous improvement (12+ months)**
- Expand monitoring and detection.  
- Review and update risk assessment annually.  
- Map progress against NIST CSF Functions for reporting.

You can use `5-maturity-roadmaps/` as your **SMB‑specific implementation plan** aligned with NIST CSF 2.0.

---

## 5. Why NIST CSF 2.0 matters for SMBs

- **Leadership language**: Functions like Govern help you explain cybersecurity to executives and boards in business terms.
- **Scalable**: Start simple, expand as you grow. No “all or nothing” requirement.  
- **Measurable**: Current Profile → Target Profile shows progress over time.  
- **Customer/partner confidence**: Many organizations ask partners to align with NIST CSF.  
- **Cyber insurance**: Many insurers expect or reward NIST CSF alignment.

NIST CSF 2.0 is **not a checklist** but a **language and structure** for organizing your security efforts. This repository provides the **practical controls** that fill in the details.

---

## 6. Minimal checklist for NIST CSF 2.0 awareness

Use this checklist to see how your current efforts align with NIST CSF 2.0:

- [ ] We have basic **governance** (roles, simple policies, roadmap).  
- [ ] We have identified our **key assets** and performed a basic **risk assessment**.  
- [ ] We have implemented core **Protect** controls (MFA, patching, backups, antivirus).  
- [ ] We have basic **Detect** capability (logging, alerts, reporting).  
- [ ] We have a **Respond** plan and **Recover** capability (playbook, tested backups).  
- [ ] We track **progress** against a simple roadmap or target profile.

This repository helps you answer “yes” to most of these over time.
