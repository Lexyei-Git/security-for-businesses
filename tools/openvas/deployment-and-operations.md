# Deployment and Operations

## Recommended SMB approach

For most SMB use cases, start with an official, well-documented installation path and avoid maintaining custom technical steps inside this repository.

A practical order is:
1. Choose an official installation path
2. Deploy on a dedicated VM or host
3. Validate service health
4. Confirm feed status
5. Start with a small pilot scan scope
6. Expand gradually

## Minimum operational flow

If using the Kali Linux package path, the official documented flow is:

1. Update the system
   - `sudo apt update && sudo apt upgrade`

2. Install Greenbone Community Edition
   - `sudo apt install gvm -y`

3. Run the setup
   - `sudo gvm-setup`

4. Verify the installation
   - `sudo gvm-check-setup`

5. Start or stop services when needed
   - `sudo gvm-start`
   - `sudo gvm-stop`

6. Confirm the feed status before the first real scan

See:
- Kali guide: https://greenbone.github.io/docs/latest/22.4/kali/index.html
- Feed sync: https://greenbone.github.io/docs/latest/22.4/source-build/feed-sync.html

## Operational cautions

- Use a dedicated host or VM for the scanner
- Do not begin by scanning the entire environment
- Validate feed readiness before scanning
- Assign ownership for triage and remediation
- Schedule scans in low-impact windows when possible
