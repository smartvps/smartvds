# Linux Administration & Web Services on Ubuntu

After establishing secure remote access, day-to-day Linux administration means understanding users and permissions, background services, resource use, and the path from an application to a public web endpoint.

This page connects five practical SmartVDS guides into a short operational learning sequence.

## 1. Learn the essential shell commands

Become comfortable navigating directories, inspecting files, reading logs, finding processes, and checking disk and memory use. Understand what each command reports before changing the system.

**Full tutorial:** [25 Ubuntu Server Commands Every Administrator Should Know](https://smartvds.org/linux/ubuntu-server-commands-guide/)

## 2. Set up users, groups, and sudo responsibly

Use separate accounts where appropriate, grant only the permissions needed for a task, and check file ownership when services cannot read configurations or write to directories. Root access and sudo should be controlled rather than shared casually.

**Full tutorial:** [How to Manage Users, Groups and Sudo Permissions on Ubuntu Server](https://smartvds.org/linux/manage-users-groups-sudo-ubuntu-server/)

## 3. Keep services under control with systemd

Learn how to check service status, start and restart units, configure automatic startup, and inspect the journal when something fails. After an application update, use its logs and dependencies to diagnose errors before repeatedly restarting the service.

**Full tutorial:** [How to Manage systemd Services on Ubuntu Server](https://smartvds.org/linux/manage-systemd-services-ubuntu-server/)

## 4. Monitor CPU, RAM, disks, and networking

Server slowness may come from resource contention, disk saturation, low storage capacity, memory pressure, or network problems. Compare system-wide counters with process-level behavior and check both available disk space and inode usage.

**Full tutorial:** [How to Monitor Ubuntu Server Performance: CPU, RAM, Disk and Network](https://smartvds.org/linux/monitor-ubuntu-server-performance/)

## 5. Publish applications with an Nginx reverse proxy

Nginx can accept client requests and forward them to a service running behind it. Correct upstream addresses, proxy headers, firewall rules, and HTTPS configuration are important for a reliable public-facing deployment. Test configuration syntax before reloading Nginx.

**Full tutorial:** [How to Install Nginx on Ubuntu Server and Configure a Reverse Proxy](https://smartvds.org/linux/install-nginx-ubuntu-server-reverse-proxy/)

## Practical maintenance routine

- Inspect service status and error logs when users report an outage.
- Check disk and inode capacity before storage or database changes.
- Review access permissions after deploying files or switching service users.
- Keep a record of Nginx configuration and verify changes before reloading.
- Maintain backups and practice restoring service configuration.

## More Linux tutorials

- [Linux Server Guides — directory](./README.md)
- [Linux security and hardening](./security-hardening.md)
- [Linux Administration & Web Services on GitBook](https://smartvds.gitbook.io/smartvds-docs/linux-guides/linux-administration)
- [SmartVDS Linux category](https://smartvds.org/category/linux/)

*Educational overview maintained as part of the SmartVDS technical knowledge resources.*
