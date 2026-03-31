# How to use this guide

This repository is designed to help small and medium businesses improve information security in a **practical and phased** way, even without a dedicated security team.

This page explains how managers and non‑security analysts can navigate the content and turn it into a concrete plan.

---

## 1. Who should read what

Different roles can use different parts of the guide:

- **Business owners and managers**
  - `0-introduction/overview.md`  
  - `1-foundations/what-is-information-security.md`  
  - `5-maturity-roadmaps/first-30-days.md`, `3-to-6-months.md`, `12-month-plan.md`  
  - `policies/README.md` and individual policy files

- **IT generalists and technical staff**
  - Everything above, plus:  
  - `1-foundations/basic-principles.md`  
  - `2-where-to-start/` (asset inventory, risk assessment)  
  - `3-practical-controls/` and `4-frameworks-explained/`

- **Non‑technical analysts (finance, HR, operations, etc.)**
  - `0-introduction/overview.md`  
  - `1-foundations/what-is-information-security.md`  
  - Selected documents from:
    - `2-where-to-start/` (especially risk assessment and 30‑day plan).  
    - `3-practical-controls/` relevant to their role (for example, email and phishing, vendor risk).

---

## 2. Recommended first‑time reading path

If you are new to this guide or to information security in general, follow this order:

1. **Understand the purpose and context**
   - Read `0-introduction/overview.md`.

2. **Learn the basics**
   - Read `1-foundations/what-is-information-security.md`.  
   - Skim `1-foundations/basic-principles.md` (confidentiality, integrity, availability, least privilege, defense in depth).

3. **Get a quick action plan**
   - Read `2-where-to-start/first-30-days.md` to see what you can accomplish in the first month.

4. **See the bigger picture**
   - Skim `5-maturity-roadmaps/3-to-6-months.md` and `12-month-plan.md` to understand how this can grow into a year‑one plan.

After this, you can dive deeper into specific controls and frameworks as needed.

---

## 3. Turning the guide into a 12‑month plan

You can use this guide as the backbone of a simple 12‑month security program:

- **Months 0–1 (First 30 days)**
  - Build a basic asset inventory (`simple-asset-inventory.md`).  
  - Run a basic risk assessment (`basic-risk-assessment.md`).  
  - Implement quick‑win controls:
    - MFA on key systems.  
    - Backups and basic restore test.  
    - Antivirus/endpoint protection.  
    - Basic phishing and password awareness.

- **Months 3–6**
  - Standardize configurations and patching (`device-hardening-and-configuration.md`, `patching-and-updates.md`).  
  - Approve and publish starter policies (`policies/`).  
  - Strengthen access control and logging.  
  - Build a simple incident response playbook (`incident-response-basics.md`).  
  - Start regular awareness and training (`security-awareness-and-training.md`).

- **Months 6–12**
  - Expand logging, monitoring and backup coverage.  
  - Improve vendor and third‑party risk management.  
  - Refine incident response and recovery testing.  
  - Define simple metrics and review them with leadership.  
  - Plan the next year using NIST CSF and CIS Controls as higher‑level references.

The roadmap files in `5-maturity-roadmaps/` provide more detail for each phase.

---

## 4. How to use the practical controls

The `3-practical-controls/` folder contains **topic‑specific guides** (for example, backups, email and phishing, Wi‑Fi and VPN, access control, cloud and SaaS security).

Use them as follows:

- When your **risk assessment** shows a priority area (for example, ransomware risk, email compromise, vendor risk), go to the relevant file:  
  - Backups → `backups.md`  
  - Email/phishing → `email-and-phishing.md`  
  - Passwords/MFA → `passwords-and-mfa.md`  
  - Wi‑Fi/VPN → `wifi-and-vpn.md`  
  - Device hardening → `device-hardening-and-configuration.md`  
  - Logging/monitoring → `logging-and-monitoring-basics.md`  
  - Vendor risk → `vendor-and-third-party-risk-basics.md`  
  - Cloud/SaaS → `cloud-and-saas-security-basics.md`

- Treat each document as:
  - A **mini‑playbook** for that control (what, why, how).  
  - A checklist to measure your current state and define next actions.

You do not need to implement everything at once: pick the controls that best address your top risks and available capacity.

---

## 5. Using frameworks without getting overwhelmed

The `4-frameworks-explained/` folder connects this guide to well‑known frameworks:

- `nist-csf-for-smbs.md`
  - Explains the NIST Cybersecurity Framework (CSF) Functions (Govern, Identify, Protect, Detect, Respond, Recover) in simple terms.  
  - Shows how the rest of this repository maps to those Functions.

- `cis-controls-for-beginners.md`
  - Summarizes the CIS Critical Security Controls and highlights which basic safeguards (Implementation Group 1) are most relevant to SMBs.  
  - Provides example mappings from `3-practical-controls/` to CIS Controls.

You can use these documents when:

- You need to **justify your approach** to management, customers or auditors.  
- You want to ensure your internal plan is roughly aligned with recognized best practices.  
- You are planning mid‑ to long‑term improvements beyond the first year.

---

## 6. How managers can drive adoption

Managers do not need to understand every technical detail, but they are crucial for making this guide real.

Key actions for managers:

- **Sponsor the effort**
  - Confirm that improving security is a business priority.  
  - Allocate time for IT and staff to work on the roadmap, not only on daily operations.

- **Approve and communicate policies**
  - Use the templates in `policies/` and follow `policies/README.md` to adapt and approve them.  
  - Ensure policies are included in onboarding and regular communications.

- **Participate in risk and incident discussions**
  - Join basic risk assessment workshops.  
  - Participate in at least one incident response tabletop exercise per year.

- **Review progress regularly**
  - Use high‑level roadmaps and simple metrics (for example, MFA coverage, backup status, awareness activities) to track progress over time.

---

## 7. If you have very limited time or resources

If you have very little time, start with **three priorities**:

1. **Protect accounts and email**
   - MFA and strong passwords on email and key systems.  
   - Basic phishing awareness.

2. **Ensure you can recover**
   - Reliable backups of critical data.  
   - At least one successful restore test.

3. **Know what to do when something goes wrong**
   - Clear incident reporting channel for staff.  
   - A short incident response checklist for phishing, malware and lost devices.

You can then gradually expand using the rest of this guide as your capacity grows.
