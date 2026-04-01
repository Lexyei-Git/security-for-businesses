# Weekly Security Review Checklist

**Week of**: ________ **Reviewer**: ________ **Duration**: 30 min

## 1. Tool Output Review (10 min)

**Nmap (network changes):**
    [ ] New hosts? Document: ________________
    [ ] Unexpected services? Investigate: ____
    [ ] Internet-facing changes? Alert IT

**ClamAV (malware):**
    [ ] Scans clean? ✅ / Threats: ____________
    [ ] freshclam updating daily? Status: ____

**OSSEC (alerts):**
    [ ] High alerts (10+): ___ Count
    [ ] All resolved? ✅ / Open: ______________
    [ ] Agent health: All connected?

**OpenVAS (if run):**
    [ ] New critical vulns? __________________
    [ ] Patches scheduled? __________________

## 2. Status Validation (10 min)

    [ ] Backups validated this month? Status: _
    [ ] Patches applied (last 2 weeks)? ______
    [ ] Incident playbooks tested? ____________
    [ ] Access reviews completed? ____________

## 3. Action Items (5 min)

**High priority (next 7 days):**
