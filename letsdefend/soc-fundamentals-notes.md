🛡️ SOC Analyst Portfolio: Let's Defend Fundamentals

This repository serves as a practical portfolio documenting my hands-on experience and investigative methodologies from the SOC Fundamentals course, specifically utilizing the Let's Defend platform's simulations.

The goal is to demonstrate proficiency in Tier 1 and Tier 2 Incident Response (IR), log analysis, and threat hunting, reinforcing skills with Linux command-line tools.

📝 Module Progress Tracker

This table tracks the completion and key takeaways from the main sections of the course.

Module / Case Study

Status

Key Focus Areas

Triage & Incident Lifecycle

✅ Completed

Alert classification, severity rating, and documentation standards.

Phishing Analysis (Email)

✅ Completed

Header inspection, decoding URLs, identifying social engineering tactics.

Web Shell / Command & Control (C2)

🛠️ In Progress

Identifying suspicious HTTP methods, rare user agents, and post-exploitation activity.

Malware File Analysis

✅ Completed

Hashing (MD5/SHA256), VirusTotal lookup, and understanding execution flow.

Linux Persistence Checks

✅ Completed

Auditing Cron jobs (crontab -l), checking system services (systemctl), and examining /etc.

🚨 Incident Response Write-Up Template

Each completed lab or incident simulation is documented in a separate markdown file (IR_\[ID]\.md). This template ensures consistency and clear communication of findings.

Case Title: [E.g., High-Severity Alert: Web Shell Detected]

Field

Detail

Incident ID

LD-2025-[ID]

Date/Time of Alert

2025-10-22 10:00:00 UTC

Security Analyst

[Your Name / GitHub Handle]

Final Status

CLOSED - True Positive (or False Positive/Escalated)

1. Initial Triage & Summary

Alert Trigger: (E.g., EDR triggered on creation of a suspicious file in /var/www/html/)

Initial Findings: A brief summary of the confirmed activity (E.g., "Confirmed creation of an anomalous file (cmd.php) used for remote command execution.")

Key Indicators of Compromise (IOCs):

Source IP: 10.10.10.5

File Hash (SHA256): a1b2c3d4e5f6g7h8...

Suspicious URL/Domain: malicious.site.com

2. Investigation & Log Analysis (CLI Focus)

Document the steps taken to validate the alert, explicitly referencing the core Linux commands you practiced.

Process Monitoring (ps, pstree): Checked for unusual parent/child relationships on the affected server. Finding: Anomalous PHP process running from web server context.

File System Audit (find, ls): Located the suspicious file and checked its metadata. Command: find /var/www/html -name 'cmd.php' -mtime -1 (Found the file created 3 hours ago).

Log Review (grep, tail): Searched the access logs for connections to the malicious file. Command: grep 'POST /cmd.php' /var/log/httpd/access.log | head -5

Persistence Check (crontab): Checked the affected user's crontab for scheduled tasks. Command: sudo crontab -l -u affected_user

3. Containment & Remediation

Containment: The host was immediately isolated via firewall rule/EDR action.

Eradication: The malicious file (cmd.php) was securely deleted, and all services were patched.

Recovery: The server was monitored for 48 hours and returned to production.

Key Takeaway: The use of grep -R was critical to quickly identify other files in the directory modified at the same time, leading to full scope of compromise.

🛠️ Core SOC & Linux Skills Demonstrated

This is the most important section for recruiters—it is a direct list of your proven capabilities.

Linux CLI Mastery (Tier 1 Focus): Highly proficient in cat, less, grep, ss, ps, tar, and find for rapid log parsing and artifact collection.

Investigation Tools (Tier 2 Focus): Practical experience with md5sum/sha256sum, strings, tcpdump, and systemctl/crontab for deep analysis and persistence checks.

Network Forensics: Analysis of packet captures (PCAP) and interpreting network connections (ss -tuln).

Incident Management: Adhering to the Incident Response Lifecycle (Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned).

Tool Familiarity: Using external tools (VirusTotal, URLScan) for threat intelligence enrichment.
