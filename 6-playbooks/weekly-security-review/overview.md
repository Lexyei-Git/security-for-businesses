# Weekly Security Review Overview

30-minute Friday routine using tools from `tools/` folder. Catches issues before they become incidents.

## When to run

**Every Friday 3PM** (30 min):
- Review tool outputs from week
- Validate alerts/actions
- Plan next week's priorities
- Document status

## Tools used

    Nmap: Network changes
    ClamAV: Malware scans
    OSSEC: Log alerts
    OpenVAS: New vulns (if scheduled)

## Review scope

    * New hosts/services (Nmap)
    * Malware detections (ClamAV)
    * High alerts (OSSEC level 10+)
    * Patch status
    * Backup validation status

## Expected outcomes

    ✅ All high alerts resolved
    ✅ New assets documented
    ✅ Next week priorities clear
    ✅ Status report generated
