# Backup Validation Checklist

**Date**: ________ **Validator**: ________ **Duration**: 60-90 min

## PHASE 1: Verify Backup Status (10 min)

    [ ] Check backup service running
    [ ] Last backup completed: _____ (within 24h)
    [ ] No errors in last 7 days
    [ ] Storage space: ___% used (alert >85%)
    [ ] Offsite sync status: Complete/In Progress

## PHASE 2: Test Critical Restores (30-45 min)

**Priority 1 - Accounting/ERP:**
    [ ] Restore 1 recent file → Verify opens correctly
    [ ] Restore 1 file from 30 days ago → Verify
    [ ] Full database backup → Test connectivity
    Time to restore: ____ minutes

**Priority 2 - Customer Data:**
    [ ] Restore sample records from 2 weeks ago
    [ ] Verify data integrity (checksum/compare)
    [ ] Test application access post-restore

**Priority 3 - Shared Files:**
    [ ] Restore 3 documents from different folders
    [ ] Verify permissions preserved
    [ ] Test shared drive mounting

## PHASE 3: Validate Offsite/DR (15 min)

    [ ] Test offsite access (VPN/cloud login)
    [ ] Verify latest backup replicated
    [ ] Test restore from offsite copy (1 file)
    [ ] Check retention: 7d/30d/90d backups present

## PHASE 4: Security & Documentation (10 min)

    [ ] Verify backup encryption enabled
    [ ] Check backup access logs (no anomalies)
    [ ] Document results:
      All pass: ✅ Complete
      Issues found: ________________________
      Action items: _______________________

## Success Criteria

    ✅ 100% critical files restorable
    ✅ RTO < 4 hours for priority 1
    ✅ Offsite backups current (<24h)
    ✅ No security issues found

**FAILURE** = Any critical system not restorable → Escalate immediately.

---
**Next run**: First Friday of next month
