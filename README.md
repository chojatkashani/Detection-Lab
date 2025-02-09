
# SIEM Deployment and Log Analysis

## Overview
This project focuses on **deploying a Security Information and Event Management (SIEM) system** using **Detection Lab** to analyze security logs, detect threats, and enhance incident response. It simulates a **real-world enterprise environment** with **Windows, Linux, and network infrastructure**, allowing hands-on experience with **log ingestion, correlation, and alerting**.

## Objectives
- Deploy and configure a **SIEM platform** (e.g., Splunk, ELK, or Graylog) in a virtualized lab.
- Collect and analyze logs from **Windows, Linux, and network devices**.
- Implement **log parsing, correlation rules, and dashboards** for security monitoring.
- Detect security incidents such as **brute force attacks, malware execution, and privilege escalation**.
- Develop **queries and alerts** for automated threat detection.
- Generate **reports for security operations** and compliance auditing.

## Lab Components
- **SIEM Platform**: Splunk, or ELK Stack.
- **Windows Infrastructure**: Windows Server, Windows 10 Workstation with Sysmon.
- **Linux Infrastructure**: Ubuntu/Debian-based system with auditd logging.
- **Network Security Tools**: Suricata IDS for network traffic analysis.
- **Log Sources**:
  - Windows Event Logs (Security, Application, System)
  - Sysmon logs (detailed process creation, network connections)
  - Linux audit logs
  - Firewall and IDS logs
  - Authentication logs (Active Directory, SSH, VPN)

## Deployment Steps
1. **Setup Detection Lab**  
   - Clone the Detection Lab repository  
   - Deploy using Vagrant & VirtualBox/VMware  
   - Configure network settings and logging agents  

2. **Install & Configure SIEM**
   - Deploy Splunk or ELK and configure indexers  
   - Install Universal Forwarders & Beats agents for log shipping  
   - Set up **log parsing and normalization** (e.g., regex, Grok patterns)  

3. **Log Collection & Forwarding**
   - Configure Windows Event Forwarding (WEF)  
   - Enable Sysmon and audit logging on Windows  
   - Configure Linux auditd and rsyslog forwarding  
   - Integrate network logs from Suricata or firewalls  

4. **Log Analysis & Threat Detection**
   - Create **SIEM correlation rules** for:
     - Failed authentication attempts (brute-force detection)  
     - Suspicious PowerShell execution  
     - Privilege escalation and lateral movement  
     - Unusual network connections  
   - Set up **SIEM dashboards** for monitoring security metrics  

5. **Incident Investigation & Response**
   - Simulate **attack scenarios** (e.g., MITRE ATT&CK techniques)  
   - Investigate alerts using **SIEM query languages** (Splunk SPL, Kibana KQL)  
   - Generate security reports and response playbooks  

## Expected Outcomes
- **Operational SIEM** with real-time log ingestion and alerting.  
- **Detection and correlation rules** to identify security threats.  
- **Comprehensive dashboards** for security event visualization.  
- **Hands-on experience** with security log analysis and investigation.  

## References
- [Detection Lab GitHub Repo](https://github.com/clong/DetectionLab)  
- [Splunk Security Essentials](https://splunkbase.splunk.com/app/3435/)  
- [Elastic Security Guide](https://www.elastic.co/guide/en/security/current/index.html)  


