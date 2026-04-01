# SMB Usage Guide

## How an SMB should use OpenVAS

OpenVAS is most useful when it is part of a repeatable review cycle instead of a one-time scan.

A simple SMB flow is:
1. Select a small group of important assets
2. Run an initial scan
3. Review the report
4. Validate critical findings
5. Assign remediation owners
6. Re-scan after changes
7. Create a recurring schedule

## Practical platform flow

According to the Greenbone scanning workflow, a basic scan usually involves:
- Creating a target
- Creating a task
- Running the task

For quick execution, the Task Wizard can be used to enter an IP address or hostname and start a scan.

Official reference:
https://docs.greenbone.net/GSM-Manual/gos-22.04/en/scanning.html

## How to read results

Reports should be used as decision support, not just as technical output.

Focus first on:
- Critical and high severity items
- Internet-facing systems
- Repeated findings
- Findings affecting business-critical servers
- Findings that can be quickly remediated

Official reference:
https://docs.greenbone.net/GSM-Manual/gos-22.04/en/reports.html

## What not to do

- Do not scan everything on day one
- Do not treat every finding as confirmed without validation
- Do not use scan output without assigning remediation ownership
- Do not rely on OpenVAS alone as your full security program
