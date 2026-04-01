# Deployment and Operations

## Installation

**Linux (Debian/Ubuntu):**
sudo apt update && sudo apt install nmap

**Linux (RHEL/CentOS/Fedora):**
sudo dnf install nmap # Fedora 22+
sudo yum install nmap # RHEL/CentOS 7

**Windows:**
Download MSI installer from https://nmap.org/download.html

**macOS:**

No server/agents needed - runs locally.

## Minimum operational flow

1. Verify installation: `nmap --version`
2. Test connectivity: `nmap scanme.nmap.org`
3. Basic network scan: `nmap 192.168.1.0/24`
4. Service scan: `nmap -sV target_ip`
5. Save output: `nmap -oN scan-results.txt target`

## SMB scan progression

1. **Host discovery**: `nmap -sn 192.168.1.0/24`
2. **Port scan**: `nmap -p- 192.168.1.0/24`
3. **Service detection**: `nmap -sV -sC target`
4. **OS detection**: `nmap -O target`
5. **Vuln scripts**: `nmap --script vuln target`

## Operational cautions

- Scans generate network traffic - test in maintenance windows
- Respect legal boundaries (your networks or authorized)
- Rate limit aggressive scans: `-T3` or `--max-rate 100`
- Document scan scope and frequency
- Review NSE script output carefully (may have false positives)
