# Linux Server Guides — Ubuntu VPS Administration

A practical, curated reading path for operating an Ubuntu VPS, VDS, or dedicated Linux server. This GitHub directory collects concise introductions to common administration topics and links directly to the full, maintained tutorials on [SmartVDS](https://smartvds.org/category/linux/).

**Start here:** [Linux Security & Hardening](./security-hardening.md) · [Linux Administration & Web Services](./administration-web-services.md) · [GitBook Linux Guides](https://smartvds.gitbook.io/smartvds-docs/linux-guides)

## What you should learn first

A new Linux server is not ready simply because you can connect by SSH. Before deploying an application, confirm that you can recover access, limit unnecessary exposure, manage administrative privileges, and observe resource usage.

| Stage | What to understand | Guide |
| --- | --- | --- |
| 1. Establish a baseline | Secure initial access and network exposure | [Ubuntu Server Security Hardening Checklist](https://smartvds.org/linux/ubuntu-server-security-hardening/) |
| 2. Protect SSH | Keys, root login, authentication and connection tests | [Secure SSH on Ubuntu Server](https://smartvds.org/linux/secure-ssh-ubuntu-server/) |
| 3. Configure the firewall | Allow necessary services while preserving SSH access | [Configure UFW Firewall](https://smartvds.org/linux/configure-ufw-firewall-ubuntu-server/) |
| 4. Control login abuse | Fail2Ban jails, logs and temporary bans | [Install and Configure Fail2Ban](https://smartvds.org/linux/install-configure-fail2ban-ubuntu-server/) |
| 5. Maintain security | Automatic package updates and review of reboots | [Automatic Security Updates](https://smartvds.org/linux/automatic-security-updates-ubuntu-server/) |
| 6. Learn the shell | Essential commands for files, processes and logs | [25 Ubuntu Server Commands](https://smartvds.org/linux/ubuntu-server-commands-guide/) |
| 7. Manage accounts | Users, groups, permissions and sudo | [Manage Users, Groups and Sudo](https://smartvds.org/linux/manage-users-groups-sudo-ubuntu-server/) |
| 8. Understand services | systemd status, startup and journal diagnostics | [Manage systemd Services](https://smartvds.org/linux/manage-systemd-services-ubuntu-server/) |
| 9. Monitor health | CPU, memory, storage and network diagnosis | [Monitor Ubuntu Server Performance](https://smartvds.org/linux/monitor-ubuntu-server-performance/) |
| 10. Deploy applications | Nginx and a reverse proxy for web services | [Install Nginx and Configure a Reverse Proxy](https://smartvds.org/linux/install-nginx-ubuntu-server-reverse-proxy/) |

## Reading paths

### [Security and hardening](./security-hardening.md)

Practical notes on SSH access, UFW, Fail2Ban, unattended security updates, and a repeatable hardening sequence.

### [Administration and web services](./administration-web-services.md)

A guide to commands, account permissions, systemd, performance monitoring, and Nginx reverse proxy basics.

## Recommended workflow

1. Confirm your operating-system release and hosting provider recovery options.
2. Read the hardening checklist and set up a non-root administrator before locking down SSH.
3. Test a new SSH connection before enabling stricter firewall rules.
4. Check logs and service health before making application changes.
5. Use the source articles for exact commands, updated screenshots, and version-specific notes.

> **Important:** These files are an educational index, not a substitute for the original tutorials or a production change plan. Commands, package versions, network interfaces, and exposed ports may differ across Linux releases and providers.

## Source and attribution

The complete and updated Linux tutorial library is available at [SmartVDS Linux Guides](https://smartvds.org/category/linux/). You can also browse the [GitBook Linux Server Guides](https://smartvds.gitbook.io/smartvds-docs/linux-guides) navigation hub.

[SmartVDS](https://smartvds.org/) is an independent server hosting catalog covering VPS/VDS, dedicated servers, and self-managed hosting tutorials.
