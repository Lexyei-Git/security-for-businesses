# SMB Usage Guide

## Basic SMB flow

**Weekly network hygiene:**
1. Map internal subnets: `nmap -sn 192.168.1.0/24`
2. Check internet-facing: `nmap your-public-ip`
3. Service inventory: `nmap -sV --top-ports 100 critical-servers`
4. Review unexpected services/versions
5. Document changes

**Monthly deep scan:**
1. Full port scan critical systems: `nmap -p- -sV critical-server`
2. Vuln check: `nmap --script vuln,smb-vuln* target`
3. OS fingerprint: `nmap -O target`
4. Save results: `nmap -oA full-scan target`

## Key SMB use cases

**Network discovery:**
   - `nmap -sn 10.0.0.0/24` # Active hosts
   - `nmap -sP --traceroute subnet` # With latency

**Service enumeration:**
   - `nmap -sV --version-intensity 9 -p 22,80,443,445 target`
   - `nmap -sV --script banner target`

**SMB/Windows specific:**
   - `nmap --script smb* -p445 target` # SMB enumeration
   - `nmap --script smb-vuln* -p445 target`

**Quick security check:**
   - `nmap -sV -sC --script vuln your-server`

## Output handling

- `-oN filename.txt` (normal)
- `-oX filename.xml` (XML for tools)
- `-oG filename.grep` (grepable)
- `-oA basename` (all formats)

## What not to do

- Never scan networks without authorization
- Don't run aggressive scans (-T5) during business hours
- Don't ignore service version findings
- Don't run without output capture
- Don't treat NSE results as confirmed vulns (validate)

Nmap excels at discovery and inventory, not replacement for vulnerability scanners.
