# Lab Journal Entry — Week 1

## 📅 Date
November 26, 2025

## 🎯 Objective
Conduct reconnaissance on the Metasploitable 2 VM using Kali Linux to identify open ports, services, and potential vulnerabilities. Document findings with screenshots and reflections for portfolio development.

---

## 🛠️ Lab Setup
- **Attacker VM:** Kali Linux (4 GB RAM, 40 GB disk, 2 CPUs)  
- **Target VM:** Metasploitable 2 (1 GB RAM, 20 GB disk, 1 CPU)  
- **Network:** Internal VirtualBox network (`LabNet`) — isolated from host internet  
- **Tools Used:** Nmap, VirtualBox snapshots, screenshot capture  

---

## 🔍 Procedure
1. Verified both VMs were connected to the `LabNet` internal network.  
2. Logged into Metasploitable 2 using default credentials (`msfadmin/msfadmin`).  
3. From Kali, ran initial scan:  
   ```bash
   nmap -A <Metasploitable_IP>
