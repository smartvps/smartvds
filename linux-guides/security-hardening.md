# Ubuntu Server Security & Hardening

Securing a Linux VPS is a series of deliberate checks rather than a single command. The objective is to reduce unnecessary exposure while keeping administrative access recoverable.

This page is a concise reading guide. The linked SmartVDS articles contain the detailed instructions and examples.

## 1. Start with a system-wide checklist

Before changing SSH or firewall settings, make sure you can access the hosting provider's recovery console or an alternative administration session. Record the Ubuntu version, current network configuration, and services that must remain reachable.

**Full tutorial:** [Ubuntu Server Security Hardening Checklist](https://smartvds.org/linux/ubuntu-server-security-hardening/)

## 2. Secure SSH without locking yourself out

Key-based authentication reduces dependence on passwords, but SSH configuration changes can interrupt remote access. Create and test the intended administrative account and public key. Check effective settings and test a second SSH connection before disabling password or root login.

**Full tutorial:** [How to Secure SSH on Ubuntu Server: Keys, Root Login and Access Settings](https://smartvds.org/linux/secure-ssh-ubuntu-server/)

## 3. Apply only the necessary firewall rules

A host firewall should allow the SSH port you actually use and only the application ports that require public access. Review the current rules and your hosting provider's additional network firewall before enabling UFW.

**Full tutorial:** [How to Configure UFW Firewall on Ubuntu Server](https://smartvds.org/linux/configure-ufw-firewall-ubuntu-server/)

## 4. Configure Fail2Ban for the services you expose

Fail2Ban monitors logs and can temporarily block IP addresses that trigger configured patterns. Its behavior depends on jail definitions, the matching log source, and the selected firewall action. Verify that expected jails are active and monitor ban events.

**Full tutorial:** [How to Install and Configure Fail2Ban on Ubuntu Server](https://smartvds.org/linux/install-configure-fail2ban-ubuntu-server/)

## 5. Plan for automatic security updates

Automatic updates help deliver security patches on time, but they do not replace log review, backups, or service-health checks. Know which packages are selected for unattended upgrades and which updates may require a reboot.

**Full tutorial:** [How to Configure Automatic Security Updates on Ubuntu Server](https://smartvds.org/linux/automatic-security-updates-ubuntu-server/)

## Suggested first-day sequence

1. Confirm a working administrator account and recovery path.
2. Review the complete hardening checklist.
3. Test key-based SSH in a second session.
4. Establish and verify firewall allow rules.
5. Enable and inspect Fail2Ban jails.
6. Configure package updates and a routine for reviewing results.

Never assume that a successful command guarantees the service is secure. Verify each change and keep a rollback option.

## More Linux tutorials

- [Linux Server Guides — directory](./README.md)
- [Linux administration and web services](./administration-web-services.md)
- [Linux Security & Hardening on GitBook](https://smartvds.gitbook.io/smartvds-docs/linux-guides/linux-security)
- [SmartVDS Linux category](https://smartvds.org/category/linux/)

*Educational overview maintained as part of the SmartVDS technical knowledge resources.*
