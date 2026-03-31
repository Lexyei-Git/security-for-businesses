# 12‑month security plan

This document outlines what a small or medium business can aim to achieve over **12 months** of focused, realistic security work.

It assumes you have followed the first 30‑day plan and the 3–6 month roadmap, and now want to **consolidate**, **measure** and **mature** your security program over the remainder of the year.

---

## 1. Starting point for the 12‑month plan

By the time you start this 12‑month view, you should already have most of the following in place:

- Asset and software inventories for key systems and data.  
- Basic risk assessment with identified high‑priority risks.  
- MFA, strong passwords and basic access control hygiene.  
- Regular patching and secure baseline configuration for endpoints and key servers.  
- Reliable backups with tested restores.  
- Antivirus/endpoint protection deployed on business devices.  
- Basic logging and monitoring for key systems and security tools.  
- Approved starter policies and a simple incident reporting process.  
- Initial vendor inventory with classification of high‑risk vendors.  
- A simple incident response playbook and at least one tabletop exercise.  
- An initial security awareness plan and one or more awareness activities.

If some items are still in progress, they become early tasks in this 12‑month window.

---

## 2. Objectives for the first year

For most SMBs, a 12‑month security plan should aim to:

1. **Stabilize and standardize** the basic controls you already introduced.  
2. **Increase coverage and completeness** of key areas (assets, logging, access, vendor risk).  
3. **Embed security into regular operations** (governance, metrics, reviews).  
4. **Strengthen detection and response** rather than relying only on prevention.  
5. **Prepare a sustainable roadmap** for the next 12–24 months based on risk and business goals.

Think of this year as moving from “ad‑hoc fixes” to a **repeatable, measured security program**.

---

## 3. Quarter 1–2 (Months 1–6): foundation and consistency

This overlaps with the earlier 3–6 month roadmap; the focus is to **finish and stabilize** foundational work.

Key outcomes:

- Asset and software inventories are reasonably complete and maintained as part of normal onboarding/offboarding.  
- Endpoint, server and network baseline configurations are documented and applied consistently.  
- Patching cycles are regular and tracked (for example, monthly reports).  
- Core policies are approved, published and referenced in onboarding.  
- High‑risk vendors have at least minimal due diligence and basic contractual expectations.  
- Staff know:
  - The basics of phishing and password hygiene.  
  - How to report incidents and to whom.

If this is not yet true, treat it as the main priority for the first half of the year.

---

## 4. Quarter 3 (Months 7–9): expand coverage and measurement

In the 7–9 month window, the focus shifts to **completeness and measurement**.

### 4.1 Close gaps in coverage

- **Assets and software**
  - Extend inventories to cover remaining devices and key applications (including remote/hybrid workers).  
  - Tag assets that are internet‑facing or especially sensitive.

- **Logging and monitoring**
  - Expand logging to more systems, such as:
    - Additional SaaS platforms.  
    - Internal applications and key network devices.  
  - Where practical, move from purely local logs to more centralised log collection.

- **Backups and recovery**
  - Ensure **all** critical systems and data (not just initial ones) have appropriate backup coverage and defined recovery objectives (for example, how much data you can afford to lose, how quickly you need to be back online).

### 4.2 Define simple metrics (KPIs/KRIs)

Create a small set of metrics to track progress and support management reporting:

Examples:

- Percentage of endpoints with:
  - Current antivirus/EDR installed and healthy.  
  - Recent patches applied (for example, last 30 days).

- Percentage of critical systems covered by:
  - Regular backups and tested restores.  
  - Logging and monitoring.

- Security awareness:
  - Number of awareness activities delivered.  
  - Phishing simulation results (if used).

- Incidents:
  - Count of reported incidents or near‑misses.  
  - Time from detection to initial response.

The goal is not perfection, but to have **consistent, repeatable measurements** that show whether things are improving.

### 4.3 Strengthen governance

- Define a **security governance cadence**:
  - For example, a short quarterly meeting where leadership reviews:
    - Top risks and any changes.  
    - Metrics and incident summaries.  
    - Roadmap progress and resource needs.

- Clarify roles:
  - Who is the security lead (even if part‑time)?  
  - Who is responsible for policies, risk assessments, vendor risk, incident management?

---

## 5. Quarter 4 (Months 10–12): optimize, test and plan next cycle

In the last quarter, focus on **testing, optimization and planning**.

### 5.1 Test your capabilities

- **Incident response**
  - Run at least one more tabletop exercise with a different scenario (for example, vendor breach or insider error).  
  - Consider a small technical test, such as:
    - Simulated account compromise.  
    - Simulated ransomware on test data.

- **Backups and recovery**
  - Perform a more realistic restore test:
    - Restore an entire small system or a representative data set.  
    - Measure time to restore and compare with business expectations.

- **Awareness**
  - Run a survey or quick feedback round to check what staff remember about:
    - Reporting incidents.  
    - Phishing indicators.  
    - Basic security responsibilities.

Document results and improvement actions.

### 5.2 Review year‑one performance

Using your metrics and logs:

- Summarize:
  - What has improved (for example, fewer high‑risk findings, faster patching, more MFA coverage).  
  - Where recurring issues remain (for example, same type of phishing incidents, gaps in vendor oversight).

- Update your **risk assessment**:
  - Re‑assess likelihood and impact of key risks.  
  - Add any new risks discovered during the year (for example, new systems, new vendors).

- Map current state to:
  - NIST CSF Functions (Govern, Identify, Protect, Detect, Respond, Recover).  
  - CIS Controls (especially IG1) to see which areas are strong or weak.

### 5.3 Build the next 12‑month roadmap

Based on the review, draft a **second‑year roadmap** (months 13–24) that might include:

- Deepening detection and response (for example, more advanced monitoring, SOC/MDR services if justified).  
- Improving application and cloud security (for example, stronger MFA and conditional access, better SaaS configuration).  
- Strengthening business continuity and disaster recovery documentation and testing.  
- Expanding coverage of CIS Controls beyond IG1 where risk justifies it.  
- Exploring more advanced concepts (for example, Zero Trust, more granular network segmentation) if appropriate for your size and industry.

The key is to keep the roadmap **realistic** and **risk‑driven**, not a long wish list.

---

## 6. Year‑one checklist

At the end of the 12‑month period, you should be able to answer “yes” to most of the following:

- [ ] We have a maintained inventory of key assets (devices, systems, data) with owners and criticality.  
- [ ] We perform a basic risk assessment at least annually, and after major changes.  
- [ ] MFA, strong passwords and basic access control hygiene are in place for key systems.  
- [ ] Endpoints, servers and key network devices follow a documented secure baseline and patching schedule.  
- [ ] Critical systems and data are backed up, and we have tested restores.  
- [ ] Antivirus/endpoint protection is deployed and monitored across business devices.  
- [ ] Logging and monitoring cover key systems, with defined responsibilities for reviewing alerts and reports.  
- [ ] Starter policies are approved, published and used in onboarding.  
- [ ] We have a simple incident response playbook and have exercised it at least twice.  
- [ ] High‑risk vendors are identified, with basic due diligence and contractual expectations recorded.  
- [ ] We have an ongoing security awareness plan and have delivered several activities.  
- [ ] We track a small set of security metrics and review them with leadership.  
- [ ] We have a documented roadmap for the next 12–24 months.

If many boxes are still unchecked, extend this 12‑month plan rather than rushing. It is better to have **fewer, well‑implemented controls** than many incomplete or poorly maintained ones.
