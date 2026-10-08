### Infrastructure / Systems Engineer
Windows & Linux · VMware vCloud Director · automation

> **🇷🇺 Кратко.** Инженер инфраструктуры: Windows Server и Linux, виртуализация на VMware vCloud Director / vCenter,
> автоматизация рутины на PowerShell, Bash и Python. Здесь — обобщённые версии моих рабочих скриптов:
> жизненный цикл ВМ, интеграция с ITSM/CMDB, мониторинг, патчинг, RDS. Все примеры обезличены.

---

**What I do**

- Automate the VM lifecycle on VMware vCloud Director / vCenter — templates, snapshots, replication, capacity and usage reports.
- Integrate infrastructure with ITSM / CMDB over REST APIs (GLPI, generic service desk APIs).
- Run monitoring with Zabbix — host lifecycle audits, templates, database health checks.
- Plan and test disaster recovery and migrations: replication, capacity checks for the recovery site.
- Patch and maintain Windows Server fleets; administer Active Directory, LAPS and Remote Desktop Services (UPD / FSLogix).

**Stack**

| Area | Tools |
|---|---|
| Scripting | PowerShell, PowerCLI, Bash, Python, REST APIs |
| Virtualization | VMware vCloud Director, vCenter, vCloud Availability, Proxmox VE |
| Windows | Windows Server, Active Directory, LAPS, RDS |
| Linux | Ubuntu, systemd, auditd |
| Monitoring & ITSM | Zabbix, GLPI |

**Repositories**

| Repository | What's inside |
|---|---|
| [rds-toolkit](https://github.com/Manick351/rds-toolkit) | RDS farms with UPD / FSLogix: profile disk inventory, compaction, cache cleanup, broken profile repair, diagnostics, helpdesk GUI |
| [windows-server-ops](https://github.com/Manick351/windows-server-ops) | Windows Server fleet: parallel patching with reboot control, LAPS/AD checks, lockout tracing, mass logoff, disk and profile cleanup, free IP search, access and Tomcat audits |
| [vmware-cloud-toolkit](https://github.com/Manick351/vmware-cloud-toolkit) | VMware Cloud Director / vCAV / vCenter: VM and capacity reports, DR readiness check, replication management, snapshots across vCenters, automated template updates |
| [itsm-cmdb-automation](https://github.com/Manick351/itsm-cmdb-automation) | GLPI CMDB, Zabbix and service desk automation: server lifecycle from tickets, inventory and monitoring sync, DNS cleanup of retired servers, ticket router, workload analytics |
| [linux-admin-scripts](https://github.com/Manick351/linux-admin-scripts) | Linux operations: hang diagnostics, AD lockout source search, Zabbix and TimescaleDB health checks, log health playbook, disk burn-in |
| [anyconnect-totp-login](https://github.com/Manick351/anyconnect-totp-login) | Cisco AnyConnect CLI login with TOTP — credentials kept in SecretManagement / DPAPI, never in plain text |

All scripts in my repositories are generalized from real-world tasks: company names, hosts, addresses and internal systems are replaced
with placeholders (`contoso.local`, `srv-app-01`, `192.0.2.x`). Most of them default to a dry run (`-WhatIf` / `--dry-run`).
