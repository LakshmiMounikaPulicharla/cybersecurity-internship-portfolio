# Task - 16 : Incident Response & Security Breach Simulation

## Project Overview
This project demonstrates a simulated security incident involving repeated failed login attempts and the complete incident response lifecycle using Linux system logs and security tools.

---

## Objectives
- Simulate a basic security breach scenario  
- Analyze authentication logs  
- Detect suspicious login activity  
- Classify and contain the incident  
- Implement preventive security measures  
- Restore system to secure operational state  

---

## Tools Used
- **Operating System:** Ubuntu Linux  
- **Logs:** Linux Authentication Logs (`/var/log/auth.log`)  
- **Services:** OpenSSH  
- **Security Tool:** Fail2Ban  
- **Utilities:** grep, tail, passwd, systemctl  

---

## Incident Scenario
A brute force login attempt was simulated by performing multiple failed SSH login attempts using incorrect credentials. Authentication logs were monitored and analyzed to detect suspicious login behavior.

---

## Implementation Steps
1. Monitored authentication logs  
2. Created a test user account  
3. Simulated multiple failed login attempts  
4. Analyzed logs to identify failed password attempts  
5. Classified the incident as brute force attack attempt  
6. Locked the affected user account  
7. Installed Fail2Ban for automatic protection  
8. Restarted and verified SSH service  

---

## Security Measures Implemented
- Account Locking using system security controls  
- Continuous Log Monitoring  
- Fail2Ban Intrusion Prevention Setup  
- SSH Service Verification  

---

## Evidence Collected
- Authentication log monitoring  
- Failed login attempts  
- Failed password log entries  
- Live log monitoring  
- Account lock confirmation  
- Login blocked verification  
- Fail2Ban active status  
- SSH service restart confirmation  

---

## Project Report
Detailed report is available in the repository: task16.pdf
