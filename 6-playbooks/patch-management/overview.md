# Patch Management Overview

Structured process to test and deploy software updates safely. Prevents "patch Tuesday disasters".

## When to run

**Bi-weekly** (2nd + 4th Tuesday):
- Test updates in staging/lab
- Deploy to production in batches
- Validate post-patch functionality
- Monitor for issues 24h after

## Patch priorities

    Priority 1: Critical security (CVSS 9.0+)
    Priority 2: High security (CVSS 7.0-8.9)
    Priority 3: Medium security + stability
    Priority 4: Feature/minor updates

## Systems covered

    * OS (server/desktop)
    * Applications (web/email/DB)
    * Network devices (firewall/switch)
    * Backup/security tools

## Team roles

    * Tester: Validates in lab
    * Deployer: Applies patches
    * Validator: Confirms functionality
    * Monitor: Watches post-deploy
