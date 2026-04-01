# Installation and Setup

## Recommended approach

For SMB environments, prefer official Greenbone Community installation methods, especially container-based deployments when possible.

This approach is generally easier to maintain and is closer to the vendor-supported community guidance than third-party package installations.

## Before deployment

Before installing OpenVAS, define:
- Where the scanner will run
- Which internal and external assets will be scanned
- Who will review the findings
- How often the vulnerability feed and scan schedules will be updated

## Basic setup considerations

- Use a dedicated scanning host or VM
- Restrict administrative access to the scanner
- Keep the vulnerability feed updated
- Document scan targets and maintenance windows
- Start with a small pilot scope before scanning the full environment
