# Backups: protecting your business data

Backups are one of the most important controls for small and medium businesses.  
If you have reliable backups, many incidents (ransomware, accidental deletion, device loss, hardware failure) become recoverable instead of catastrophic.

This document explains, in practical terms, what you need to know and what you should do to set up and maintain business‑grade backups.

---

## 1. Objectives of a backup strategy

A good backup strategy for a small or medium business should:

- Ensure you can recover important data and systems after an incident (for example, ransomware, hardware failure, theft, fire, or user error).
- Keep at least one copy of important data **physically or logically separated** from your main systems (off‑site or in the cloud).
- Encrypt backups and limit access so that only authorized people can read or restore them.
- Be **tested regularly**, so you know that restores actually work.

---

## 2. What needs to be backed up

You do not need to back up everything at the same level. Focus on what you cannot afford to lose.

Typical categories:

- **Business‑critical data**
  - Accounting and finance data
  - Customer records and CRM data
  - Contracts, proposals, legal documents
  - Key operational data (orders, production, projects)

- **Important shared content**
  - Shared file repositories and team folders
  - Documentation, procedures and internal knowledge bases

- **Key systems and configurations**
  - Configuration of servers, network devices and critical applications
  - Databases that support business processes

For each item, decide:

- **How quickly** you need it back (hours, days).  
- **How much data loss** you can tolerate (for example, losing one day of changes vs. one week).  

These answers drive backup **frequency** and **type**.

---

## 3. The 3‑2‑1 rule (simple design)

A simple way to think about backup design is the **3‑2‑1 rule**:

- **3 copies** of your important data  
  - 1 primary (the one you use)  
  - + at least 2 backup copies  

- **2 different types of storage**  
  - For example: local network storage (NAS or external drive) **and** cloud backup.

- **1 copy off‑site**  
  - For example: backup in a reputable cloud provider or at a different physical location.

For many small businesses, a realistic setup is:

- Local backup (for fast restore) **plus**  
- Cloud backup (for off‑site, disaster and ransomware resilience).

---

## 4. Backup types (keep it simple)

From a non‑specialist perspective, you mainly need to understand:

- **Full backup**  
  - A complete copy of the selected data.  
  - Slower and larger, but easy to understand and restore.

- **Incremental backup**  
  - Only copies changes since the last backup.  
  - More efficient, but restore may require combining multiple backup points.

For small businesses using modern backup software or cloud backup:

- Configure at least:
  - Periodic **full backups** (for example, weekly).  
  - More frequent **incremental backups** (for example, daily between full backups).

If your solution hides these details and just says “continuous backup” or “daily backup”, that is acceptable as long as:

- Backups run automatically.  
- Multiple restore points are available.  

---

## 5. Backup locations: local and cloud

### 5.1 Local backups

Examples: NAS device in the office, external hard drive connected to a server or workstation.

Advantages:

- Fast backup and restore.  
- Works even with limited internet bandwidth.

Risks:

- Vulnerable to theft, fire, flood or physical damage.  
- If permanently connected to the network, can be encrypted by ransomware together with the primary data.

### 5.2 Cloud backups

Examples: cloud backup services, storage from reputable providers, backup features integrated in major SaaS products.

Advantages:

- Off‑site by design (protects against physical incidents at your office).  
- Often includes versioning and geographic redundancy.  
- Accessible from different locations if your primary site is unavailable.

Considerations:

- Check **where** the data is stored (country/region) and any regulatory impact.  
- Ensure data is **encrypted in transit and at rest**, and that you control access.

---

## 6. Frequency and retention

You should define, at minimum:

- **Backup frequency** – how often backups run.
  - Many small businesses aim for **daily** backups of critical data.
  - Some very small environments may accept **weekly** backups, but daily is safer.

- **Retention period** – how long you keep old backup versions.
  - Example: keep daily backups for 30 days, weekly backups for 3 months, monthly backups for 1 year.
  - Longer retention helps recover from issues discovered late (for example, data quietly corrupted weeks ago).

Keep this simple and document it in 4–5 lines so everyone knows the expectation.

---

## 7. Security of backups

Backups must be protected almost as carefully as the original data.

Key points:

- **Encryption**
  - Ensure backups are encrypted in storage (at rest) and during transmission (in transit).
  - For physical media, enable disk encryption (for example, BitLocker, FileVault) or use backup software that encrypts backup files.

- **Access control**
  - Limit access to backup systems and media to a small set of authorized people (for example, IT administrator, trusted service provider). 
  - Use strong authentication and, where possible, multi‑factor authentication.

- **Isolation from ransomware**
  - Keep at least one backup copy that is **not directly writable** from everyday user accounts and servers (for example, cloud backup with immutable or versioned storage, offline copies).
  - Avoid having the only backup permanently mounted as a normal drive on the same network where ransomware can reach it.

---

## 8. Testing restores (do not skip this)

Backups that are never tested are a common failure point.

At least:

1. **Define what to test**
   - For example: restore a single file, restore a folder, or restore a small test database.

2. **Test on a regular schedule**
   - Example: perform a small restore test **at least quarterly**.  
   - After major changes (for example, new backup software), run an extra test.

3. **Document results**
   - Note date, what was restored, how long it took and any issues found.  
   - Use these results to improve procedures or adjust retention.

4. **Update procedures**
   - If a restore fails or is slower than your business can tolerate, adjust your approach (more frequent backups, different storage, improved documentation).

---

## 9. Roles and responsibilities

For small and medium businesses, clarity about “who does what” is critical.

Typical roles:

- **Backup owner**
  - Usually an IT lead, managed service provider, or a designated technical contact.  
  - Responsible for designing the backup approach, configuring tools and maintaining documentation.

- **Backup operator**
  - Executes routine tasks: checking backup status, swapping physical media if used, running restore tests.  
  - May be the same person as the backup owner in small organizations.

- **Business owner(s) of data**
  - Finance, HR, Sales, Operations, etc.  
  - Responsible for confirming that backups cover the data they need and that retention periods align with their requirements.

Make these responsibilities explicit in a short internal note or policy.

---

## 10. Minimal checklist for small and medium businesses

Use this as a quick review checklist:

- [ ] We have identified our critical data, systems and locations.  
- [ ] We back up critical data **at least daily** (or at a frequency that matches our risk tolerance).  
- [ ] We have **at least two backup copies**, and at least one copy is off‑site or in the cloud.  
- [ ] Backups are **encrypted** and access to them is restricted.  
- [ ] At least one backup copy is protected from direct modification by normal users and systems (for example, offline, immutable or logically isolated).  
- [ ] We have a simple, written description of our backup frequency and retention.  
- [ ] We **regularly test** restores and record the results.  
- [ ] We know who is responsible for managing backups and who to contact in case of an incident.

If you cannot yet check all boxes, use this list to prioritize your next improvements.
