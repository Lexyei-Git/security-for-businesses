# Basic cyber risk assessment

This document describes a simple, repeatable way for small and medium businesses to perform a **basic cyber risk assessment**.

It is designed for non‑security analysts: you do not need advanced tools or methodologies. You just need a clear list of your assets, your main threats, and a simple way to rate and prioritize risks.

You can use the CSV template in `templates/basic-risk-assessment.csv` as a starting point for your risk register and adapt the columns to your needs.

---

## 1. What a basic risk assessment is (and is not)

A basic cyber risk assessment for this guide is:

- A **short, structured exercise** to understand:
  - What you are trying to protect (assets).  
  - What could go wrong (threats and vulnerabilities).  
  - How bad it would be (impact).  
  - How likely it is over the next 1–2 years (likelihood).  
  - What you should focus on first (priorities).

It is **not**:

- A formal, heavily quantitative risk model.  
- A one‑time project that never gets updated.

For most SMBs, a basic risk assessment should fit on a few pages or a simple spreadsheet (for example, `templates/basic-risk-assessment.csv`) and be updated at least once a year, or when major changes occur.

---

## 2. Who should be involved

For a small or medium business, keep the group small but representative:

- A **business lead or manager** who understands priorities and consequences.  
- Someone responsible for **IT / systems** (internal or external provider).  
- Optionally, a **front‑line staff member** who knows day‑to‑day workflows.

Aim to complete a first pass in **one or two short workshops** (for example, 1–2 hours each), plus some follow‑up to finalize notes.

---

## 3. Step 1 – List your key assets

Start by listing the **assets** you want to protect:

- **Systems and infrastructure**
  - Email and collaboration (for example, Microsoft 365, Google Workspace).  
  - File storage and document management (on‑premises or cloud).  
  - Line‑of‑business applications (ERP, CRM, HR, industry‑specific tools).  
  - Websites, e‑commerce platforms and customer portals.  
  - Network infrastructure (routers, firewalls, Wi‑Fi, VPN).

- **Data**
  - Customer data.  
  - Financial and accounting records.  
  - Employee and HR data.  
  - Intellectual property and product designs.  
  - Operational data (orders, inventory, production, service delivery).

- **People and processes**
  - Key roles (finance, sales, operations, HR, IT).  
  - Critical manual processes (for example, payment approvals, order fulfillment).

Use your asset inventory (for example, the file `templates/asset-inventory.csv`) as the basis for this step.

---

## 4. Step 2 – Identify common threat scenarios

Next, think about **what could go wrong** for your assets. Focus on common, realistic scenarios for SMBs.

Examples:

- **Business email compromise**
  - Attackers gain access to a mailbox and use it to change payment instructions or impersonate staff.

- **Ransomware**
  - Malware encrypts files on servers, laptops or cloud storage, demanding payment to restore them.

- **Data breach in a cloud service**
  - Misconfiguration or vendor incident exposes customer or employee data.

- **Lost or stolen device**
  - A laptop or phone with access to business systems is lost or stolen.

- **Insider error**
  - Staff accidentally send sensitive data to the wrong recipient or make a misconfiguration that exposes data.

- **Third‑party compromise**
  - A vendor with access to your systems or data is breached and attackers pivot to your environment.

You do not need to list every theoretical threat. Start with 5–10 realistic scenarios that match your business and industry.

---

## 5. Step 3 – Rate likelihood and impact (simple scale)

For each **asset–threat** combination that feels relevant, estimate:

- **Likelihood** – how likely is this scenario in the next 1–2 years?  
- **Impact** – how bad would it be for your business if it happened?

Use a simple 3‑level scale to keep it understandable:

- Likelihood: **Low / Medium / High**  
- Impact: **Low / Medium / High**

Questions to help with impact:

- Would this stop us from operating for hours, days or more?  
- Would it involve sensitive customer or employee data?  
- Would we have to notify customers, regulators or the public?  
- How much would it cost in money, time and reputation?

You can put this in a small table or use the `templates/basic-risk-assessment.csv` file with columns such as:

| Asset / Process             | Threat scenario           | Likelihood | Impact | Notes                         |
|-----------------------------|---------------------------|-----------|--------|-------------------------------|
| Email and collaboration     | Business email compromise | High      | High   | Payment fraud, data exposure  |
| Shared file storage         | Ransomware                | Medium    | High   | Operations blocked for days   |
| Customer database (CRM)     | Cloud misconfiguration    | Medium    | High   | Privacy incident, notifications |
| Finance systems             | Lost laptop               | Low       | Medium | Encrypted, but still disruptive |

---

## 6. Step 4 – Decide which risks matter most

Combine likelihood and impact to decide **overall priority**:

- **High priority**
  - High impact and medium or high likelihood.  
  - These should receive attention **first**.

- **Medium priority**
  - Medium impact and/or medium likelihood.  
  - Address after high‑priority items.

- **Low priority**
  - Low impact and low likelihood.  
  - May be accepted or handled later.

You can visualize this in a simple 3×3 matrix or just add a “Priority: High/Medium/Low” column in `templates/basic-risk-assessment.csv`.

At the end of this step, you should have:

- A short list of **high‑priority risks** to address.  
- A longer list of medium and low risks to consider later.

---

## 7. Step 5 – Link risks to practical controls

For each **high‑priority risk**, decide which **controls** (actions) from this repository can reduce likelihood or impact.

Examples:

- Risk: business email compromise  
  - Controls:
    - `passwords-and-mfa.md` – strong authentication on email.  
    - `email-and-phishing.md` – staff training and email security.  
    - `logging-and-monitoring-basics.md` – watch for unusual login patterns.

- Risk: ransomware on shared files  
  - Controls:
    - `backups.md` – reliable, tested backups.  
    - `patching-and-updates.md` – reduce vulnerabilities.  
    - `antivirus-and-anti-malware.md` – detect and block malware.  
    - `device-hardening-and-configuration.md` – limit spread and impact.

- Risk: data breach in a cloud service  
  - Controls:
    - `access-control-basics.md` – least privilege and proper account management.  
    - `wifi-and-vpn.md` – secure remote access.  
    - `vendor-and-third-party-risk-basics.md` – better selection and oversight of vendors.

For each high‑priority risk, write down in `templates/basic-risk-assessment.csv`:

- Which controls you **already have**.  
- Which controls you **plan to implement or improve**, and in what timeframe.

This becomes the start of your **action plan**.

---

## 8. Step 6 – Document and revisit

Your basic risk assessment does not need to be long, but it should be **written down**:

Include, for example in `templates/basic-risk-assessment.csv`:

- The date and people involved.  
- The list of key assets and scenarios.  
- The risk ratings (likelihood, impact, priority).  
- The list of chosen controls and actions.

Revisit this assessment:

- **At least annually**, or  
- When there are major changes (for example, new systems, mergers, big shifts to cloud or remote work), or  
- After a security incident or near‑miss.

Each new iteration should be easier, because the structure is already in place.

---

## 9. Minimal checklist for a basic risk assessment

Use this checklist to see whether you have completed a usable basic risk assessment:

- [ ] We have a short, written list of our key systems, data and processes (for example, in `templates/asset-inventory.csv`).  
- [ ] We have identified realistic threat scenarios that could affect our business.  
- [ ] We have rated likelihood and impact for major risks using a simple scale.  
- [ ] We have identified which risks are high, medium and low priority.  
- [ ] We have linked high‑priority risks to specific controls and actions in this guide.  
- [ ] We have recorded who participated and when the assessment was done.  
- [ ] We have decided how often we will review and update the assessment.

If several boxes are unchecked, use this document and the template `templates/basic-risk-assessment.csv` to complete a first assessment and turn it into a repeatable habit, not a one‑time exercise.
