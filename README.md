# Information and Cyber Security Guide for Small and Medium Businesses

This repository is a practical, plain‑language guide to help small and medium businesses improve their cyber security, even if they do not have a dedicated security team.

It is written for non‑security analysts and managers who need to understand **what to do**, **why it matters**, and **how to implement basic controls step by step**.

---

## Who this guide is for

- Small and medium businesses (SMBs/SMEs), especially in Canada.  
- IT generalists and system administrators.  
- Business professionals in risk, compliance, finance, HR, operations and other areas who are responsible for security tasks but are not security experts.  
- Security professionals who need clear, non‑technical material to explain security to business stakeholders.

---

## What you will find here

- **Foundations** – simple explanations of core information security concepts.  
- **Where to start** – a basic risk assessment approach, a simple asset inventory and a 30‑day action plan.  
- **Practical controls** – focused guides on concrete controls (backups, patching, passwords and MFA, email and phishing, Wi‑Fi/VPN, device hardening, logging, vendor risk, etc.).  
- **Frameworks explained** – plain‑English introductions to the NIST Cybersecurity Framework and CIS Critical Security Controls, tailored for SMBs.  
- **Policies** – starter policy templates managers can adapt and approve.  
- **Roadmaps** (planned) – suggested 3–6 month and 12‑month improvement plans.


The goal is to bridge the gap between **high‑level frameworks** and **day‑to‑day actions** in a small or medium business.

---

## Repository structure

High‑level structure (folders link to sub‑content):

- `0-introduction/`  
  - `overview.md` – why this guide exists and how it is organized.

- `1-foundations/`  
  - `what-is-information-security.md` – business‑friendly definition and context.  
  - `basic-principles.md` – confidentiality, integrity, availability (CIA) and other key principles.

- `2-where-to-start/`  
  - `first-30-days.md` – 30‑day “quick win” action plan.  
  - `simple-asset-inventory.md` – guidance for building a basic asset inventory.  
  - `basic-risk-assessment.md` – simple, repeatable risk assessment approach.  
  - `starter-policies-and-templates.md` – overview of essential starter policies.

- `3-practical-controls/` (examples, not exhaustive)  
  - `backups.md`  
  - `passwords-and-mfa.md`  
  - `email-and-phishing.md`  
  - `patching-and-updates.md`  
  - `antivirus-and-anti-malware.md`  
  - `access-control-basics.md`  
  - `wifi-and-vpn.md`  
  - `device-hardening-and-configuration.md`  
  - `logging-and-monitoring-basics.md`  
  - `physical-security-basics.md`  
  - `vendor-and-third-party-risk-basics.md`

- `4-frameworks-explained/`  
  - `nist-csf-for-smbs.md` – NIST Cybersecurity Framework explained for SMBs.  
  - `cis-controls-for-beginners.md` – CIS Critical Security Controls explained for beginners and SMBs.

- `5-maturity-roadmaps/` (planned)  
  - `first-30-days.md` – tactical checklist (linked from `2-where-to-start/`).  
  - `3-to-6-months.md` (planned).  
  - `12-month-plan.md` (planned).

- `policies/`  
  - `acceptable-use-policy.md`  
  - `passwords-and-mfa-policy.md`  
  - `backup-and-data-protection-policy.md`  
  - `email-internet-and-phishing-policy.md`  
  - `incident-reporting-policy.md`  
  - `vendor-and-third-party-security-policy.md`  
  - `README.md` – how managers should choose, adapt and approve policies.
 
- `templates/`  
  - `asset-inventory.csv` – basic inventory of devices, systems, applications and key data sets.
  - `basic-risk-assessment.csv` – simple risk register linking assets to threats, likelihood, impact and planned controls.
  - `vendor-inventory-and-assessment.csv` – vendor and third-party inventory with a basic security risk view.
  - `incident-log.csv` – log for security incidents and near-misses, including containment, lessons learned and follow-up actions.
  
---

## How to get started (recommended path)

If you are new to information security in your organization:

1. **Read the overview**  
   - Start with `0-introduction/overview.md` to understand the purpose and scope of this guide.

2. **Learn the basics**  
   - Read `1-foundations/what-is-information-security.md` and `basic-principles.md` to get core concepts (CIA triad, least privilege, defense in depth).

3. **Understand your environment**  
   - Use `2-where-to-start/simple-asset-inventory.md` to list your key systems, data and processes.  
   - Use `2-where-to-start/basic-risk-assessment.md` to identify and prioritize your main risks.

4. **Act in the first 30 days**  
   - Follow `2-where-to-start/first-30-days.md` for a practical sequence of quick‑win actions.

5. **Implement key controls**  
   - Work through the relevant documents in `3-practical-controls/` (backups, patching, passwords/MFA, email/phishing, Wi‑Fi/VPN, etc.) to address your highest‑priority risks.

6. **Formalize expectations with policies**  
   - Use the templates in `policies/` and the guidance in `policies/README.md` to create and approve simple, realistic policies.

7. **Connect to frameworks (optional but recommended)**  
   - When you need to explain your approach to management, customers or auditors, use:
     - `4-frameworks-explained/nist-csf-for-smbs.md` as your high‑level map.  
     - `4-frameworks-explained/cis-controls-for-beginners.md` as your tactical checklist reference.

---

## Relationship to NIST CSF and CIS Controls

This repository is designed to align with widely used frameworks while staying pragmatic for small and medium businesses:

- **NIST Cybersecurity Framework (CSF)**  
  - `nist-csf-for-smbs.md` explains the six Functions (Govern, Identify, Protect, Detect, Respond, Recover) in plain language and shows where the content of this repo fits.

- **CIS Critical Security Controls (CIS Controls)**  
  - `cis-controls-for-beginners.md` describes the CIS Controls and highlights which IG1 (basic) safeguards are most relevant to SMBs.  
  - Many documents in `3-practical-controls/` map directly to IG1 safeguards (for example, assets, secure configuration, backups, malware defenses, access control, logging, vendor risk).

You can say, for example:

> “Our security program is based on the NIST Cybersecurity Framework, and we use the CIS Critical Security Controls (Implementation Group 1) as a practical checklist for the controls we implement.”

---

The long‑term intention is for this repository to be a **living reference** for organizations that need to improve their security posture step by step, without assuming deep security expertise or large budgets.
