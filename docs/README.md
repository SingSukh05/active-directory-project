# Active Directory Project

An interactive, single-page report documenting a hands-on Active Directory home-lab
project, built and troubleshooted end to end across six phases:

1. **Design & Network** — network diagram, VMs, NAT network, static IPs (Netplan), shared storage
2. **Splunk & Sysmon** — SIEM install, Universal Forwarder + Sysmon on every Windows host, logs on :9997
3. **Active Directory** — promote the domain controller, OUs, users, DNS, domain join
4. **Validation & Atomic Red** — controlled brute force (Crowbar/RDP), detection in Splunk (Event 4625/4624),
   adversary emulation with Atomic Red Team mapped to MITRE ATT&CK
5. **Hardening** — group-based permissions, logon-hour restrictions, automatic account expiration
6. **Troubleshooting** — account lockouts, recurring lockouts (Event Viewer source-tracing),
   expired accounts, HR permission gaps, broken workstation trust relationship

## View it locally

Open `index.html` in any browser. Everything is self-contained — one HTML file plus the
`screenshots/` folder, no build step.

## Publish free on GitHub Pages

1. Create a new GitHub repo and push these files (keep `index.html` and `screenshots/` together).
2. In the repo: **Settings → Pages → Build and deployment**.
3. Source: **Deploy from a branch**. Branch **main**, folder **/docs**
   (or **/ (root)** if these files live at the repo root).
4. Save — your report goes live at `https://<your-username>.github.io/<repo>/`.
