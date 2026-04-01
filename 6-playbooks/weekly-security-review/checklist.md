# Weekly Security Review Checklist

**Week of**: ________ **Reviewer**: ________ **Duration**: 30 min

## 1. Tool Output Review (10 min)

**Nmap (network changes):**
- [ ] New hosts? Document: `________________`
- [ ] Unexpected services? Investigate: `____`
- [ ] Internet-facing changes? Alert IT

**ClamAV (malware):**
- [ ] Scans clean? ✅ / Threats: `____________`
- [ ] freshclam updating daily? Status: `____`

**OSSEC (alerts):**
- [ ] High alerts (10+): `___` count
- [ ] All resolved? ✅ / Open: `______________`
- [ ] Agent health: All connected?

**OpenVAS (if scans ran this week):**
- [ ] New critical findings? `______________`
- [ ] Remediation owner assigned? `__________`

## 2. Status Validation (10 min)

- [ ] Backups validated this month? Status: `___`
- [ ] Patches applied in last 2 weeks? Status: `___`
- [ ] Incident playbooks tested recently? `Yes/No`
- [ ] Access reviews completed for admins? `Yes/No`

## 3. Action Items (5 min)

**High priority (next 7 days):**
1. `________________________________` Owner: `___`
2. `________________________________` Owner: `___`
3. `________________________________` Owner: `___`

## 4. Documentation (5 min)

**Status summary for this week:**

- 🔴 **RED** – Immediate action needed  
- 🟡 **YELLOW** – Issues identified, scheduled for next week  
- 🟢 **GREEN** – All systems normal, no outstanding high‑risk items

**Send summary to:** IT team + management (email or chat)  
**Next review:** Next Friday at 15:00
