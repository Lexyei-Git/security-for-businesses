# Templates

This folder contains simple templates (mainly CSV files) that small and medium businesses can use to **kick‑start documentation and record‑keeping** for their security program.

The goal is to give you practical, lightweight tools you can open in Excel, Google Sheets or any spreadsheet editor, without requiring specialized software or complex formats.

---

## 1. Files in this folder

Current templates:

- `asset-inventory.csv`  
  Basic asset inventory for devices, systems, applications and key data sets.

- `basic-risk-assessment.csv`  
  Simple risk register linking assets to threat scenarios, with likelihood/impact ratings and planned controls.

- `vendor-inventory-and-assessment.csv`  
  Vendor and third‑party inventory with a high‑level security and risk view.

- `incident-log.csv`  
  Incident tracking log for recording security incidents and near‑misses.

You can download these files and edit them locally, or open and edit them directly in GitHub’s web interface.

---

## 2. How to use the templates

### 2.1 General tips

- Treat these files as **starting points**, not final designs.  
- Add or remove columns to match your environment, but keep them **consistent** over time.  
- Use them together with:
  - `2-where-to-start/simple-asset-inventory.md`  
  - `2-where-to-start/basic-risk-assessment.md`  
  - `3-practical-controls/vendor-and-third-party-risk-basics.md`  
  - `3-practical-controls/incident-response-basics.md`

You can convert the CSV files to `.xlsx` or Google Sheets if that is easier for your team.

---

## 3. Asset inventory – `asset-inventory.csv`

This file helps you answer: **“What do we actually have?”**

Use it to:

- List key **devices, systems and data sets** that support your business.  
- Record who is responsible for each asset.  
- Mark which assets are critical, handle personal/sensitive data or are internet‑facing.

Suggested steps:

1. Start with your most critical systems (email, file storage, CRM, finance, HR, key SaaS).  
2. Fill in a row for each asset using the header fields.  
3. Update the inventory when new systems are added or old ones are retired.

This template supports your **risk assessment, patching, backup planning and incident response**.

---

## 4. Basic risk assessment – `basic-risk-assessment.csv`

This file is a simple **risk register**.

Use it to:

- Link each important asset to realistic **threat scenarios** (for example, phishing, ransomware, lost laptop).  
- Rate **likelihood** and **impact** using a Low/Medium/High scale.  
- Decide **overall priority** for each risk.  
- Record existing and planned controls and who is responsible for implementing them.

Suggested steps:

1. Take your asset inventory and identify 5–10 key risks.  
2. Add one row per risk with a short description and ratings.  
3. Link planned controls back to the relevant documents in `3-practical-controls/`.  
4. Review and update at least once per year, or after major changes or incidents.

---

## 5. Vendor inventory & assessment – `vendor-inventory-and-assessment.csv`

This file helps you manage **third‑party and SaaS risk**.

Use it to:

- List vendors and service providers that store your data or have access to your systems.  
- Capture what services they provide and what data they process.  
- Classify vendors by **risk level** (High/Medium/Low).  
- Track basic security due diligence and whether contracts include security/privacy clauses.

Suggested steps:

1. List your most important SaaS platforms, MSP/MSSP partners and other critical vendors.  
2. For each, fill in what they do, what data they see, and what access they have.  
3. Mark high‑risk vendors and perform basic security checks for them.  
4. Review high‑risk vendors at least annually.

---

## 6. Incident log – `incident-log.csv`

This file is for recording **security incidents and near‑misses**.

Use it to:

- Capture basic facts about each incident (what happened, when, who reported it).  
- Track containment, root cause, impact and notifications.  
- Record lessons learned and follow‑up improvement actions.

Suggested steps:

1. Each time you have a suspected or confirmed incident, add a row.  
2. Update the row as you learn more (root cause, impact, actions).  
3. Use the log in your **post‑incident reviews** and annual risk assessments.

Over time, this log helps you see patterns (for example, repeated phishing issues) and justify improvements.

---

## 7. Adapting templates to your organization

You are encouraged to adapt these templates:

- Add fields that are important for your context (for example, regulation tags, data classification, project codes).  
- Remove fields you will never use to keep the templates simple.  
- If you have a more advanced tool (for example, ticketing system, GRC tool), you can use these CSVs as an **import starting point**.

The most important thing is not perfection, but that:

- The templates are **actually used**, and  
- They are **kept up‑to‑date enough** to support decisions and improvements.

---
The long‑term intention is for this repository to be a living reference for organizations that need to improve their security posture step by step, without assuming deep security expertise or large budgets.
