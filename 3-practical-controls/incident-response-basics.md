# Incident response basics

Even with good prevention controls, incidents will still happen.  
Incident response is about **reacting quickly and effectively** when something goes wrong so you can limit damage, recover faster and learn from the event.

This document provides a simple, practical incident response approach for small and medium businesses.

You can use the `templates/incident-log.csv` to track and document incidents and near‑misses over time.

---

## 1. What is an incident (plain language)

A **security incident** is any event that:

- Actually harms, or
- Could reasonably harm

the **confidentiality, integrity or availability** of your systems, data or services.

Examples include:

- A user clicks a phishing link and enters their password on a fake page.  
- Malware or ransomware is detected on a device.  
- A laptop with company data is lost or stolen.  
- A vendor informs you of a breach affecting your data.  
- Sensitive information is emailed to the wrong recipient.

Your incident response approach should cover both confirmed incidents and strong suspicions (for example, “I think I entered my password on a fake site”).

---

## 2. Goals of incident response for SMBs

For a small or medium business, incident response aims to:

- **Protect people and safety first.**  
- **Contain** the incident quickly so it does not spread or get worse.  
- **Restore** critical services and data as soon as practical.  
- **Communicate** clearly with staff, customers, vendors and regulators as required.  
- **Learn** from the incident to reduce the chance and impact of future events.

You do not need a complex playbook; you need a **short, clear plan** that people can follow under pressure.

---

## 3. Roles and responsibilities (keep it simple)

Define roles by **function**, not just by name, so your plan still works if people change.

Typical roles in a small or medium business:

- **Incident lead / coordinator**
  - Usually an IT lead, security champion or operational manager.  
  - Responsible for coordinating the response and making decisions.

- **Technical responder(s)**
  - Internal IT staff and/or external service provider (MSP/MSSP).  
  - Handle containment, investigation and recovery steps on systems.

- **Business owner(s)**
  - Managers responsible for affected areas (for example, Finance, HR, Operations).  
  - Help prioritize which services and data must be restored first.

- **Communications / management**
  - Leadership or designated spokesperson.  
  - Handles external communication (customers, partners, regulators, media) where necessary.

Make these roles explicit in your incident response playbook and ensure people know **how to reach each role**, including after hours if needed.

---

## 4. Simple 6‑step incident response cycle

For SMBs, a straightforward cycle works best:

1. **Identify** – Notice and confirm that something is wrong.  
2. **Contain** – Stop the incident from spreading or getting worse.  
3. **Eradicate** – Remove the cause (for example, malware, compromised account).  
4. **Recover** – Restore systems and data, return to normal operations.  
5. **Communicate** – Inform the right people at the right time.  
6. **Learn** – Review what happened and improve controls and processes.

You can map these to NIST CSF **Detect**, **Respond** and **Recover** Functions, but the steps above should be kept in plain language in your playbook.

---

## 5. Playbook templates for common scenarios

Below are high‑level playbook outlines for three common scenarios. You can adapt and expand these in a separate internal document.

### 5.1 Phishing / suspected credential theft

**Example:** A user clicked a phishing link and entered their password.

1. **Identify**
   - User reports the incident or email security flags it.  
   - Incident lead logs basic details (who, when, which account, what was clicked) in `templates/incident-log.csv`.

2. **Contain**
   - Immediately change the user’s password.  
   - Invalidate sessions/tokens for that account where possible.  
   - If MFA is not enabled, enable it; if it is, check for unusual approvals.

3. **Eradicate**
   - Ensure the phishing email is removed from other mailboxes if possible (for example, using email admin tools).  
   - Block the malicious domain or URL at email / web filtering level.

4. **Recover**
   - Confirm the user can log in normally with the new credentials.  
   - Check if any sensitive actions were taken from the account (for example, forwarding rules, password resets, data downloads).

5. **Communicate**
   - Inform impacted managers as needed.  
   - Share an anonymized example with staff as a learning opportunity.

6. **Learn**
   - Update phishing training materials with this example.  
   - Review whether email filtering or MFA coverage needs improvement.

### 5.2 Malware / ransomware on a device

**Example:** Endpoint protection detects ransomware on a workstation.

1. **Identify**
   - Alert received from endpoint protection, user reports unusual behavior (files encrypted, ransom note, system slow).

2. **Contain**
   - Disconnect the affected device from the network (unplug cable / disable Wi‑Fi).  
   - Do not power off unless instructed by your incident lead or support provider.

3. **Eradicate**
   - Technical responder investigates:
     - Confirm type of malware.  
     - Remove or isolate malware using security tools or re‑imaging.

4. **Recover**
   - Restore affected files or systems from clean backups where necessary.  
   - Verify that restored systems are functioning correctly.

5. **Communicate**
   - Inform relevant business owners and management.  
   - If customer or employee data might be affected, involve legal/privacy contacts to assess notification requirements.

6. **Learn**
   - Review how the malware entered (for example, phishing, unpatched system, removable media).  
   - Strengthen controls (email filtering, patching, endpoint protection, user awareness) as needed.

### 5.3 Lost or stolen device

**Example:** A laptop with access to email and internal systems is stolen.

1. **Identify**
   - User reports laptop lost or stolen (where, when, any details).

2. **Contain**
   - Use device management tools to:
     - Attempt remote lock or wipe, if available.  
     - Remove the device from allowed device lists.

3. **Eradicate**
   - Change passwords for user accounts accessible from the device.  
   - Invalidate authentication tokens for email and other critical systems.

4. **Recover**
   - Provide a replacement device after ensuring the account is safe.  
   - Restore any necessary local data from backups or cloud storage if available.

5. **Communicate**
   - Inform IT, management and, if appropriate, legal/privacy contacts.  
   - Evaluate whether regulatory or contractual notifications are required if sensitive data was stored unencrypted on the device.

6. **Learn**
   - Confirm disk encryption and screen lock policies on all portable devices.  
   - Review physical security and user training related to device handling.

---

## 6. Integrating policies, logs and backups

Your incident response basics depend heavily on other controls:

- **Policies**
  - `incident-reporting-policy.md` tells staff **what to report** and **how**.  
  - Acceptable use, email/internet and vendor policies define expected behavior and responsibilities.

- **Logging and monitoring**
  - `logging-and-monitoring-basics.md` ensures you have the logs needed to investigate (for example, logins, admin changes, malware alerts).

- **Backups**
  - `backups.md` provides the foundation for recovery after data loss or ransomware.

Make sure your incident playbook **references where logs are stored**, how to access them and which backups to use in specific scenarios.

---

## 7. Documentation and evidence

Even a small organization should **document** incidents and responses using `templates/incident-log.csv`:

- For each incident:
  - Short description (what happened, when, who was involved).  
  - Actions taken (containment, eradication, recovery).  
  - Any notifications made (customers, regulators, vendors).  
  - Lessons learned and follow‑up actions.

- Store incident records:
  - In a central, access‑controlled location (for example, ticketing system, secure shared folder).  
  - With enough detail to support future investigations or audits.

This documentation helps you:

- Show due diligence to management, partners or regulators.  
- Avoid repeating the same mistakes.  
- Improve your risk assessment and controls over time.

---

## 8. Minimal checklist for incident response basics

Use this checklist to evaluate your current readiness:

- [ ] We have defined who leads incident response and who is involved (IT, management, business owners).  
- [ ] We have a short, written incident response playbook that covers at least phishing, malware/ransomware and lost/stolen devices.  
- [ ] Staff know **what** to report and **how** to report suspected incidents.  
- [ ] We know where key logs are stored and who can access them during an incident.  
- [ ] We have tested at least one incident scenario through a tabletop exercise.  
- [ ] We document incidents (even small ones) and track lessons learned and follow‑up actions using `templates/incident-log.csv`.  
- [ ] Incident response is discussed periodically with management as part of our overall security governance.

If several boxes are unchecked, use this document as a starting point to build and refine your incident response capability over the next 3–12 months.
