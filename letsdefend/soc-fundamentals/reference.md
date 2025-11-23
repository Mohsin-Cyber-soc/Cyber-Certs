# SOC Fundamentals – Reference Guide

## 🧰 Tools & Concepts Cheat Sheet  
- **SIEM**: Collects & correlates logs from multiple sources; generates alerts for SOC analysts.  
- **EDR**: Endpoint Detection & Response — monitors endpoint devices for malicious or anomalous activity.  
- **SOAR**: Security Orchestration, Automation & Response — automates repetitive SOC workflows and incident handling.  
- **Log Management**: Centralised collection and analysis of logs from endpoints, servers, network devices, firewalls.  
- **Threat Intelligence Feed**: Provides indicators (IPs, domains, hashes) and reputation data for proactive detection.  

## 📚 Key References  
- Course Table of Contents: Introduction to SOC; SOC Types & Roles; SOC Analyst Responsibilities; SIEM & Analyst Relationship; Log Management; EDR; SOAR; Threat Intelligence Feed; Common Mistakes. :contentReference[oaicite:10]{index=10}  
- Blog/Write‑up on the course structure: “LetsDefend | SOC Fundamentals Training” (Medium). :contentReference[oaicite:11]{index=11}  

## ✅ Best Practices from Course  
- Always verify alerts: not every alert is an incident. Use tool data + context.  
- Use logging consistently: a SOC is only as good as the log sources it monitors.  
- Keep EDR telemetry and endpoint investigations in mind — many threats start on endpoints.  
- Automate repetitive tasks with SOAR to free up time for deeper analysis.  
- Use threat intelligence feeds selectively: integrate relevant indicators, but don’t rely exclusively on them.  
- Document your investigations and refine processes: avoid falling into alert fatigue or “checking boxes”.  

## 🔍 Practical Reference Tips  
- Create quick search queries in your SIEM for common event types (e.g., failed logins, unusual process creations).  
- Write down key Linux/Windows commands you use in investigations (e.g., `netstat`, `tasklist`, `grep`, `Get-EventLog`).  
- Maintain a personal list of commonly seen Alerts → Investigation steps → Response.  
- Keep a “common mistakes” log: whenever you make a mistake, note what it was and how you’ll avoid it next time.  

> **Tip:** Use this reference guide anytime you review your notes, practice in labs, or prepare for interviews. It’s your quick‑reference toolkit for SOC fundamentals.
