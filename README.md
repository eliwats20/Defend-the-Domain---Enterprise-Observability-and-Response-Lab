# Defend the Domain - Enterprise Observability and Response Lab
Cybersecurity home lab for Active Directory, Kali Linux attacks, SIEM monitoring, log correlation, and incident response exercises.

## 🛠️ Tools Used

- **Windows Server 2022** – Active Directory Domain Services (AD DS), DNS, Sysmon
- **Windows 10 Client** – Domain-joined endpoint for attack simulation
- **Kali Linux** – Offensive security tools (`nmap`, `hydra`, `metasploit-framework`)
- **Elastic Stack (ELK)** – Elasticsearch, Logstash, Kibana, Elastic Defend (SIEM)
- **Winlogbeat** – Forwards Windows Event Logs (including Sysmon) to Elastic
- **Sysmon** – Captures detailed Windows telemetry (process creation, network connections, etc.)

---

## 📋 Prerequisites

Before running this lab, ensure the following:

- ✅ Virtualization platform (e.g., VirtualBox, VMware Workstation, or Hyper-V)
- ✅ At least **16 GB RAM** and **100 GB disk space** (recommended for smooth VM performance)
- ✅ Internet access for package installation and updates
- ✅ Basic networking setup (e.g., internal NAT or bridged adapter for VM communication)
- ✅ Elastic Stack installed and configured (can be on a separate VM or cloud instance)
- ✅ Winlogbeat and Sysmon installed and configured on Windows machines
- ✅ Kali Linux updated with necessary tools:
  ```bash
  sudo apt update && sudo apt install nmap hydra metasploit-framework

## Steps

1. **Setup Active Directory (AD)**
   - Install the AD DS role on Windows Server 2022
   - Promote the server to a domain controller (e.g., `corp.local`)
   - Create user accounts and organizational units (OUs)
<img width="374" height="265" alt="image" src="https://github.com/user-attachments/assets/1d3c9cec-dc2e-41cc-ab14-35d0a4d2fc03" />

