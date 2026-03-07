# Prower

> A self-built homelab server used to practice and document real-world DevOps workflows.
>
> *Lovingly named after Tails "Miles" Prower from Sonic the Hedgehog.*

---

## What is Prower?

Prower is a personal homelab server running Proxmox, built and maintained since November 2025. It hosts a mix of VMs and containers that I build, break, harden, and document - the same way you would in a professional environment.

This isn't a sandbox that's just spun up and forgotten. Everything on Prower gets real use, real monitoring, and real incident response. If something breaks, there's a log for it. If it isn't used, it's deprecated to save resources.

---

## Why Does This Exist

I've spent ~6 years in IT and the thing I've consistently wanted more of is the ability to actually *build* - to automate the repetitive, to provision infrastructure with a single command, and to make systems that just work without someone having to babysit them.

DevOps is where that happens. It's where I want to be, and Prower is how I get there, by doing it on myself, documenting it properly, and treating a homelab like production infrastructure.

---

## What's Running

| Name | Type | Role | Status |
|---|---|---|---|
| Infrastructure-VM-01 | VM | Primary automation and control node | Running |
| Monitoring-VM-01 | VM | Prometheus, Grafana, Node Exporter, Alertmanager | Running|
| CEJ-CT | Container | Self-hosted Minecraft server | Running |
| MCTestBranch | Container | Sandboxed test environment for CEJ | Planned |

---

## Current Stack
- **Hypervisor:** Proxmox VE
- **OS:** Ubuntu Server 24.04 LTS (VMs), Debian 12 (Containers)
- **Containers:** Docker + Docker Compose
- **Monitoring:** Prometheus, Grafana, Node Exporter, Alertmanager
- **Security:** UFW, Fail2ban, SSH key-only authentication, unattended upgrades
- **IaC (in progress):** Terraform, Ansible
- **CI/CD (in progress):** GitHub Actions

---

## What I'm Practicing

- Infrastructure as Code - Automated VM and container provisioning with Terraform and Ansible
- Observability - Metrics, dashboards, and email alerting with Prometheus and Grafana
- Security hardening - Firewall rules, Intrusion prevention, and SSH hardening on every node
- Incident response - Real postmortems and incident reports written to professional standards
- Documentation - Every change, problem, and resolution is logged the way it should be in a real ops environment

---

## The Full Picture

All changes, build logs, incident reports, and postmortems live in the companion repo:

### [Prower-Progress-Logs](https://github.com/SpiritCreations/Prower-Progress-Logs)

If this README is the cover letter, that repo is the portfolio.

---

*Built and maintained by [SpiritCreations](https://github.com/SpiritCreations)*
