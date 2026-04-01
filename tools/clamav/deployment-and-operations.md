# Deployment and Operations

## Installation (Linux)

**Debian/Ubuntu:**
   - `sudo apt update`
   - `sudo apt install clamav clamav-daemon clamav-freshclam`
   - `sudo freshclam # Initial signature update`

**RHEL/CentOS/Rocky:**
   - `sudo dnf install clamav clamav-update`
   - `sudo freshclam`

**Windows/macOS:**
Download from https://www.clamav.net/downloads

## Minimum operational flow

1. **Update signatures**: `sudo freshclam`
2. **On-demand scan**: `clamscan -r /path/to/scan`
3. **Daemon scan**: `clamdscan -r /path`
4. **Quick file check**: `clamscan file.txt`
5. **System-wide**: `clamscan -r --bell -i /`

## Start daemon (recommended)
   - `sudo systemctl start clamav-daemon`
   - `sudo systemctl enable clamav-daemon`
   - `sudo systemctl status clamav-daemon`

## Scheduled scans (cron)
## Daily full scan
   - `0 2 * * * /usr/bin/clamscan -r --bell -i / >> /var/log/clamav/scan.log`

## SMB progression

1. **Signatures**: Automate `freshclam` daily
2. **Manual scans**: Test directories/files
3. **Daemon mode**: Enable `clamd` for performance
4. **Mail integration**: Add `clamav-milter` for Postfix
5. **Scheduled**: Cron full system weekly

## Operational cautions

- Signatures need daily updates (automate)
- First `freshclam` download can take 30+ minutes
- Scans are CPU/disk intensive (schedule off-hours)
- False positives possible (review logs)
- Monitor `/var/log/clamav/clamd.log`
