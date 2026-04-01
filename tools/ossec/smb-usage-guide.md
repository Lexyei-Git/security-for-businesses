# SMB Usage Guide

## Basic SMB flow

1. Deploy server on stable host
2. Install agents on critical servers/workstations
3. Configure log collection for key sources (auth, syslogs, app logs)
4. Enable FIM on important directories (/etc, /bin)
5. Set up email alerts for level 10+
6. Review daily alerts
7. Weekly FIM report review
8. Monthly agent health check

## Key features for SMB

- File integrity monitoring (FIM) on config files and binaries
- Log analysis for authentication failures, service starts/stops
- Rootkit detection
- Policy monitoring (permissions, users)
- Active response (block IPs after failed logins)

## Common configurations

Monitor these logs by default:
- /var/log/auth.log
- /var/log/secure  
- /var/log/messages
- Windows event logs (via agent)

## What not to do

- Do not deploy without email alerts configured
- Do not ignore agent connectivity issues
- Do not disable default rules without testing
- Do not treat all alerts as critical without review
- Do not use as sole security control

Consider Wazuh fork for dashboard, API, and easier management.
