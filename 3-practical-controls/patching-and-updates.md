# Patching and updates

Keeping systems and applications up to date is one of the most important security actions a business can take.  
Most successful attacks exploit vulnerabilities in software that could have been fixed by applying available patches or updates.

This document explains, in practical terms, what patching is, why it matters for small and medium businesses, and how to organize a simple, repeatable process.

---

## 1. What patching is (in business terms)

A **patch** or **update** is a change to software or firmware that:

- Fixes security vulnerabilities.  
- Fixes bugs that affect stability or performance.  
- Sometimes adds or changes features.

Patching and updates apply to:

- Operating systems (for example, Windows, macOS, Linux, mobile OS).  
- Applications (office suites, browsers, PDF readers, line‑of‑business applications).  
- Servers, network devices and security appliances (for example, firewalls, routers, VPN gateways).

---

## 2. Why patching matters for SMBs

Unpatched systems are one of the most common ways attackers get into organizations of all sizes.

For small and medium businesses:

- Attackers often scan the internet for systems with known vulnerabilities and then automatically try to exploit them.  
- Publicly known vulnerabilities are widely documented, and exploit code is often available.  
- Many ransomware and data breach incidents are traced back to unpatched operating systems, servers, VPN devices or internet‑facing applications.

Patching reduces the “window of opportunity” for attackers and is consistently ranked as a top security action in government and industry guidance.

---

## 3. Scope: what should be patched

At a minimum, your patching scope should include:

- **Endpoints**
  - Desktop and laptop operating systems.  
  - Common applications (browsers, office suites, PDF readers, email clients, collaboration tools).

- **Servers**
  - Operating systems (on‑premises or cloud).  
  - Application servers, database servers, file servers.

- **Network and security devices**
  - Firewalls, routers, VPN devices, Wi‑Fi access points, security appliances.

- **Business‑critical applications**
  - Accounting/ERP, CRM, HR systems, industry‑specific applications.

Also track:

- **End‑of‑life (EOL) software** – systems and applications that are no longer supported by the vendor and do not receive security updates. These should be replaced or isolated as soon as possible.

An accurate, up‑to‑date **asset inventory** (list of systems and applications) is critical so you know what needs to be patched.

---

## 4. Basic patching principles for SMBs

For a small or medium business, the patching process does not need to be complex, but it should follow a few principles:

- **Prioritize security patches**
  - Treat security patches differently from pure feature updates.  
  - High‑severity security fixes for internet‑facing or critical systems should be prioritized.

- **Patch early and patch regularly**
  - Do not wait months to apply security updates.  
  - Have a defined schedule (for example, monthly) plus the ability to handle urgent patches faster.

- **Test when risk is high**
  - For critical servers and business‑critical applications, test patches in a small group or non‑production environment before broad deployment, when possible.

- **Automate where practical**
  - Use automatic updates and patch management tools to reduce manual work and missed systems.

- **Document and monitor**
  - Keep simple records of patch status and key decisions.  
  - Periodically check that systems are still receiving updates as expected.

---

## 5. Simple patching process (step by step)

A reasonable patching process for a small or medium business can be broken into steps:

1. **Identify what needs updates**
   - Maintain a list of your operating systems, applications and devices.  
   - Use built‑in tools, patch management software or vulnerability scanners where available.

2. **Monitor for new patches**
   - Subscribe to vendor notifications for key products (for example, Microsoft, Apple, major line‑of‑business software).  
   - Regularly check your patch management dashboard or update console.

3. **Assess and prioritize**
   - Prioritize patches that:
     - Fix critical or high‑severity security vulnerabilities.  
     - Affect internet‑facing or externally accessible systems.  
     - Protect high‑value or sensitive data.

4. **Test (when appropriate)**
   - For servers and critical applications:
     - Apply patches to a small number of systems first (pilot group).  
     - Verify that key business functions still work.

5. **Deploy updates**
   - Roll out updates during defined **maintenance windows** to reduce business impact.  
   - Use automated tools or centralized management where possible.

6. **Verify and monitor**
   - Confirm that patches have been applied successfully (for example, by checking version numbers or compliance reports).  
   - Investigate and resolve failed installations.

7. **Document**
   - Keep a simple record of:
     - What was patched.  
     - When it was patched.  
     - Any issues and how they were resolved.

---

## 6. Frequency and timelines

You should define clear expectations for **how quickly** different types of patches are applied.

A practical approach:

- **Routine schedule**
  - For most systems, apply updates on a **monthly** cycle (for example, a specific week each month).  
  - Workstations and non‑critical servers can often be updated more frequently using automatic updates.

- **Security‑critical patches**
  - For security updates rated critical or high severity on important systems:
    - Aim to deploy within **days or a couple of weeks**, depending on risk and testing needs.  
    - Internet‑facing systems and remote access devices may need faster action.

- **Emergency patches**
  - For widely exploited or extremely severe vulnerabilities:
    - Be prepared to apply patches **out of cycle**, potentially within 24–48 hours, with minimal testing.  
    - Have an emergency procedure and communication plan for this scenario.

Align these timelines with your organization’s risk tolerance and business impact.

---

## 7. Automation and tools

Manually patching each device and server does not scale and leads to gaps.

Where possible, use:

- **Built‑in automatic updates**
  - Enable automatic updates for operating systems and widely used applications on endpoints, where business risk is low.

- **Centralized patch management**
  - Use endpoint management or patch management tools to:
    - See which systems are missing patches.  
    - Approve and deploy patches in groups.  
    - Generate simple compliance reports.

- **Cloud and SaaS updates**
  - Many cloud services (for example, SaaS applications) are updated automatically by the provider.  
  - Your responsibility is to stay informed about major changes and adjust configurations if needed.

Even with automation, you still need **human oversight** to confirm that everything is working and critical systems have not been missed.

---

## 8. Handling systems that cannot be patched

Some systems cannot be updated easily (for example, legacy applications, devices with vendor‑locked firmware, unsupported operating systems).

For these, consider **compensating controls**:

- Isolate them on separate network segments with strict access controls.  
- Limit which users and systems can communicate with them.  
- Add extra monitoring and logging.  
- Plan to replace or upgrade them as soon as practical.

Document any unpatchable systems along with the risk and compensating controls applied.

---

## 9. Roles and responsibilities

For patching to work, people need to know what they are responsible for.

Typical assignments in a small or medium business:

- **Patch management owner**
  - Defines the patching approach, schedule and priorities.  
  - Often an internal IT lead or external managed service provider.

- **System administrators**
  - Apply patches to servers, network devices and critical applications.  
  - Test key systems after updates.

- **Endpoint support**
  - Ensure workstations and laptops are updated (via centralized tools or automatic updates).  
  - Help users with update‑related issues.

- **Business owners**
  - Confirm acceptable maintenance windows.  
  - Validate that key business functions continue to work after patching.

Make these responsibilities visible in a short internal document or policy.

---

## 10. Minimal checklist for patching and updates

Use this checklist as a quick status check:

- [ ] We maintain an inventory of our key systems, applications and devices.  
- [ ] We have a defined schedule for routine updates (for example, monthly patching cycle).  
- [ ] We prioritize security patches, especially for internet‑facing and business‑critical systems.  
- [ ] Automatic updates are enabled where appropriate (especially on workstations).  
- [ ] We use some form of centralized or automated patch management (where feasible).  
- [ ] We test patches for critical systems before broad deployment when possible.  
- [ ] We have a process for emergency patching when severe vulnerabilities are announced.  
- [ ] We document patching activities and monitor for systems that are falling behind.  
- [ ] We have identified any systems that cannot be patched and applied compensating controls.

If multiple boxes are unchecked, treat them as priorities for your next 30–90 days of security improvement work.
