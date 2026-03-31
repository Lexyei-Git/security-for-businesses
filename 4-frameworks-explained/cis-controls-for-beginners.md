# CIS Critical Security Controls for beginners

The CIS Critical Security Controls (CIS Controls) are a prioritized list of security practices created to help organizations defend against the most common cyberattacks.

This document explains the CIS Controls in simple terms and shows how small and medium businesses (SMBs) can use them, especially the parts that matter most at the beginning.

---

## 1. What the CIS Controls are (plain language)

The CIS Controls are:

- A set of **18 high‑level security controls**, maintained by the Center for Internet Security (CIS).  
- Broken down into many smaller, actionable **Safeguards** (sub‑controls).  
- Designed to be **prioritized**, so you do not try to do everything at once.

Key ideas:

- They focus on **real‑world attack patterns**, not theory.  
- They are meant to be **practical for SMBs**, especially through **Implementation Group 1 (IG1)**, which is tailored to organizations with limited resources.

---

## 2. Implementation Groups (IG1, IG2, IG3) explained simply

CIS Controls are organized into three **Implementation Groups (IGs)**:

- **IG1 – Basic cyber hygiene**
  - Designed for most small and medium businesses.  
  - Focuses on essential safeguards that stop the most common attacks.  
  - Can be implemented with limited staff and budget.

- **IG2 – Intermediate level**
  - Builds on IG1 for organizations with higher risk or regulatory expectations.  
  - Adds more monitoring, response and governance activities.

- **IG3 – Advanced level**
  - For complex, high‑risk environments (for example, critical infrastructure, heavily regulated sectors).  
  - Includes the full set of safeguards and more advanced capabilities.

For this repository and for many SMBs, **IG1 is the main focus**.  
You can treat IG1 as a practical “to‑do list” for foundational security.

---

## 3. Overview of the 18 CIS Controls

CIS Controls v8/v8.1 define 18 top‑level Controls.

In simplified terms:

1. **Inventory and Control of Enterprise Assets**  
   Know which devices (laptops, desktops, servers, network gear) you have and control their access.

2. **Inventory and Control of Software Assets**  
   Know which software you have installed and control what is allowed.

3. **Data Protection**  
   Protect sensitive data in transit, at rest and in use (encryption, access controls, backups).

4. **Secure Configuration of Enterprise Assets and Software**  
   Harden devices and applications with secure, standardized settings.

5. **Account Management**  
   Manage user accounts and identities consistently across systems.

6. **Access Control Management**  
   Ensure only the right people can access the right systems and data (least privilege).

7. **Continuous Vulnerability Management**  
   Identify and address vulnerabilities in systems and applications.

8. **Audit Log Management**  
   Collect and review logs to detect suspicious activity.

9. **Email and Web Browser Protections**  
   Reduce risks from phishing, malicious websites and browser‑based attacks.

10. **Malware Defenses**  
    Detect and respond to malicious software on endpoints.

11. **Data Recovery**  
    Ensure you can restore data and systems from backups.

12. **Network Infrastructure Management**  
    Secure and manage routers, switches, firewalls and other network devices.

13. **Network Monitoring and Defense**  
    Monitor network traffic and detect anomalies or intrusions.

14. **Security Awareness and Skills Training**  
    Train staff to recognize and respond to common threats.

15. **Service Provider Management**  
    Manage cyber risk from vendors and third parties.

16. **Application Software Security**  
    Build and acquire software with security in mind.

17. **Incident Response Management**  
    Plan, prepare and execute responses to security incidents.

18. **Penetration Testing**  
    Test defenses with controlled, simulated attacks.

You do **not** need to implement all 18 Controls fully to see benefits.  
Most SMBs should start with the **IG1 safeguards** within the Controls that matter most for their environment.

---

## 4. Which CIS Controls matter most for SMBs (IG1 focus)

Different sources highlight slightly different priority sets, but for most SMBs the following Controls (at IG1 level) are especially important:

- **CIS Control 1 – Inventory and Control of Enterprise Assets**  
- **CIS Control 2 – Inventory and Control of Software Assets**  
- **CIS Control 3 – Data Protection**  
- **CIS Control 4 – Secure Configuration of Enterprise Assets and Software**  
- **CIS Control 5 – Account Management**  
- **CIS Control 6 – Access Control Management**  
- **CIS Control 7/9 – Email and Web Browser Protections** (numbering varies by summary)  
- **CIS Control 8/10 – Malware Defenses**  
- **CIS Control 11 – Data Recovery**  
- **CIS Control 14 – Security Awareness and Skills Training**  
- **CIS Control 15 – Service Provider Management**

In plain language, IG1 for SMBs usually means:

- Know your devices and software.  
- Harden and patch them.  
- Protect accounts and access.  
- Defend against phishing and malware.  
- Back up and recover data.  
- Train your people.  
- Manage vendor risk.

These areas map very closely to the practical controls in this repository.

---

## 5. How this repository maps to CIS Controls (examples)

The practical controls you have in `3-practical-controls/` already align with many IG1 safeguards.

Example mappings:

| Repository control                                      | CIS Controls (approximate)           |
|---------------------------------------------------------|--------------------------------------|
| `device-hardening-and-configuration.md`                 | 1 – Assets, 4 – Secure Configuration |
| `patching-and-updates.md`                               | 7 – Continuous Vulnerability Management, 4 – Configuration |
| `antivirus-and-anti-malware.md`                         | 8/10 – Malware Defenses              |
| `passwords-and-mfa.md`                                  | 5 – Account Management, 6 – Access Control |
| `access-control-basics.md`                              | 5 – Account Management, 6 – Access Control, 3 – Data Protection |
| `backups.md`                                            | 3 – Data Protection, 11 – Data Recovery |
| `email-and-phishing.md`                                 | 9 – Email and Web Browser Protections, 14 – Security Awareness |
| `wifi-and-vpn.md`                                       | 1 – Assets, 12 – Network Infrastructure, 13 – Network Monitoring & Defense |
| `logging-and-monitoring-basics.md`                      | 8 – Audit Log Management, 13 – Network Monitoring & Defense |
| `physical-security-basics.md`                           | 3 – Data Protection (physical aspects), supports multiple controls |
| `vendor-and-third-party-risk-basics.md`                 | 15 – Service Provider Management     |

This table is approximate, but it shows that your practical guidance already supports a large part of CIS IG1 in a language suitable for non‑specialists.

---

## 6. How SMBs can start with CIS Controls in practice

A simple, phased approach for SMBs:

1. **Identify your Implementation Group**
   - Most small and medium businesses should assume **IG1** as their starting point.  
   - Confirm that you do not have special regulatory or threat conditions that would push you toward IG2 or IG3.

2. **Perform a light CIS IG1 assessment**
   - Use publicly available IG1 checklists or tools (for example, CIS IG1 worksheets) to see which safeguards you already have and which are missing.
   - Do not overcomplicate: a simple “yes / no / partial” view is enough to begin.

3. **Prioritize high‑impact safeguards**
   - Focus first on:
     - Asset and software inventory (Controls 1–2).  
     - Secure configuration and patching (Controls 4 and 7).  
     - Account and access control with MFA (Controls 5–6).  
     - Malware defenses and email/browser protections (Controls 8–9).  
     - Backups and recovery (Control 11).  
     - Security awareness and vendor management (Controls 14–15).

4. **Use existing content in this repository**
   - For many IG1 safeguards, you can point directly to the relevant “practical controls” documents as your implementation guidance for non‑security staff.

5. **Document progress**
   - Track which safeguards you have implemented and when.  
   - Use a simple spreadsheet or checklist; this also helps with client and auditor questions.

---

## 7. Relationship between CIS Controls and NIST CSF

CIS Controls and the NIST Cybersecurity Framework (NIST CSF) are **compatible**, not competing frameworks.

- NIST CSF provides a **high‑level structure** (Govern, Identify, Protect, Detect, Respond, Recover).  
- CIS Controls provide **detailed, prioritized safeguards** that map into those Functions.

For SMBs:

- You can use NIST CSF in `nist-csf-for-smbs.md` as your **strategic map**.  
- You can use CIS Controls (especially IG1) as your **tactical checklist** of concrete actions.

This repository is designed so that:

- The **Foundations** and **Frameworks Explained** sections align with NIST CSF.  
- The **Practical Controls** section lines up with many CIS IG1 safeguards.

---

## 8. How to talk about CIS Controls to non‑specialist stakeholders

When explaining your approach to management, clients or partners, you can say something like:

> “We are using the CIS Critical Security Controls as a practical checklist to improve our security. We focus on Implementation Group 1 (IG1), which is specifically designed for small and medium businesses. Many of our policies and how‑to guides are aligned with these controls, so non‑security staff know exactly what to do.”

This keeps the language business‑friendly, while still showing alignment with a recognized, data‑driven security framework that is widely recommended for SMBs.
