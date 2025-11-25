# Case Study: Metasploitable 2 Vulnerability Analysis

## 📅 Date
November 25, 2025

## 🎯 Objective
To identify, exploit, and document vulnerabilities within the Metasploitable 2 virtual machine, simulating a real-world penetration test and forensic investigation.

---

## 🛠️ Lab Setup
- **Attacker VM:** Kali Linux (latest build)  
- **Target VM:** Metasploitable 2 (Ubuntu-based vulnerable system)  
- **Network:** Internal lab-only network (isolated from home internet)  
- **Tools Used:** Nmap, Metasploit Framework, Wireshark, Autopsy  

---

## 🔍 Procedure
1. **Reconnaissance:**  
   - Ran `nmap -A <target IP>` to identify open ports and services.  
   - Discovered vulnerable FTP and outdated Apache web server.  

2. **Exploitation:**  
   - Used Metasploit to exploit vsftpd backdoor vulnerability.  
   - Gained shell access to the target system.  

3. **Evidence Collection:**  
   - Captured network traffic with Wireshark during exploitation.  
   - Created forensic disk image using FTK Imager for later analysis.  

4. **Analysis:**  
   - Examined logs and file system with Autopsy.  
   - Identified malicious processes and weak configurations.  

---

## 📈 Findings
- Multiple critical vulnerabilities (FTP backdoor, weak MySQL credentials).  
- Exploitation allowed full system compromise.  
- Forensic evidence confirmed insecure configurations and lack of monitoring.  

---

## 💡 Reflection
This exercise reinforced the importance of:
- **Reconnaissance:** Thorough scanning reveals the attack surface.  
- **Documentation:** Screenshots and logs are critical for forensic reporting.  
- **Defense-in-Depth:** Even basic monitoring could have detected the intrusion.  

---

## 📎 Supporting Materials
- [Screenshots](../Screenshots/) of Nmap results, exploitation, and forensic analysis.  
- [Network Diagram](../Network-Diagrams/lab-layout.png) showing attacker/target setup.  

---

> *“Every vulnerability tells a story — the analyst’s job is to document it clearly and learn from it.”*
