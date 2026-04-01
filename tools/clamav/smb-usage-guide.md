# SMB Usage Guide

## Basic SMB flow

**Daily:**
- `sudo freshclam # Update signatures`

**Weekly:**
**Scan critical directories**
- `clamscan -r --bell -i /home /var/www /shared-files`

**Or daemon mode (faster)**
- `clamdscan -r --bell -i /home /var/www`

**Monthly full scan:**
- `clamscan -r --bell -i / >> /var/log/clamav/monthly-scan.log`

## Key SMB use cases

**File server protection:**
- `clamscan -r /srv/files --move=/quarantine`

**Web uploads:**
- `clamscan --stream < uploaded-file`

**Mail gateway (with Postfix):**
- `clamav-milter integration`
- `clamdscan -c /etc/clamav/clamd.conf`

**Quick file check:**
- `clamscan document.pdf # Single file`
- `echo "threats found: $(clamscan file | grep Infected)"`

**Automated upload scanning:**
- `#!/bin/bash`

- `scan-uploads.sh`
- `freshclam`
- `clamscan --no-summary -i "$1" || echo "INFECTED: $1" | mail -s "Malware found" admin@company.com`

## Common configurations

**freshclam.conf (updates):**
- `DatabaseMirror database.clamav.net`
- `Checks 24`

**clamd.conf (daemon):**
- `MaxConnectionQueueLength 30`
- `MaxThreads 20`

## Output analysis

**Clean**
   - `/home/user/file: OK`

**Infected**
/home/user/malware.exe FOUND: Eicar-Test-File

## What not to do

- Never skip signature updates
- Don't scan during business hours (CPU intensive)
- Don't ignore "Heuristics" or "PUP" detections without review
- Don't run without log capture
- Don't treat as complete endpoint protection (use with other controls)

ClamAV excels at signature-based malware detection, not behavioral analysis or zero-day protection.
