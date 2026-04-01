# Patch Management Checklist

**Cycle**: 2nd/4th Tuesday **Deployer**: ________ **Duration**: 2-4 hours

## PHASE 1: Preparation (30 min)

    [ ] Review advisories:
        * OpenVAS critical findings
        * Vendor security bulletins
        * CISA/US-CERT Known Exploited

    [ ] Inventory systems:
        Count: ___ servers + ___ workstations + ___ network devices

    [ ] Staging environment ready? (VM/test server)

## PHASE 2: Test Phase (60-90 min)

**Priority 1 patches:**
    [ ] Download: ________________________
    [ ] Test in staging: Services start? Apps work?
    [ ] Rollback test successful
    [ ] Document compatibility

**Batch production:**
    Group 1: 20% critical systems
    Group 2: 40% secondary systems  
    Group 3: 40% low-risk systems

## PHASE 3: Deployment (60-90 min)

**Batch 1 (20%):**
    [ ] Pre-backup configs/databases
    [ ] Apply patches
    [ ] Reboot/service restart
    [ ] Verify: nmap ports + app access

**Batch 2+3**: Same process, staggered 30min apart

## PHASE 4: Validation + Monitor (ongoing)

**Immediate (1h post-deploy):**
    [ ] All services responding
    [ ] No critical alerts (OSSEC)
    [ ] Business functions OK

**24h monitoring:**
    [ ] Log review (OSSEC/clamav)
    [ ] Performance baseline check
    [ ] User feedback collection

## Success Criteria

    ✅ 100% Priority 1 patched
    ✅ <5% rollback needed
    ✅ All services functional post-patch
    ✅ No new critical vulns (OpenVAS re-scan)

**FAILURE** = Service outage >30min → Rollback + analyze

---
**Next cycle**: 2 weeks
