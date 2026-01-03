# 1. Alert Priority Levels
## Core Concepts
### Priority Definitions
Alert priority levels are used to determine how urgently a security alert must be handled based on impact and risk.

- Critical: An immediate and severe threat that can cause major damage, such as ransomware encryption or active exploitation of a critical vulnerability.
- High: A serious threat like unauthorized administrator access where damage is possible but not yet confirmed.
- Medium: Suspicious activity that requires investigation, such as repeated failed login attempts or brute-force attacks.
- Low: Informational or low-risk activity such as port scans or policy violations without immediate threat.

### Assignment Criteria
Alerts are prioritized using multiple factors:

- Asset Criticality: Production servers and business-critical systems have higher priority than test or lab systems.
- Exploit Likelihood: Vulnerabilities with publicly available exploits are more dangerous.
- Business Impact: Potential data loss, service downtime, or financial damage increases priority.
- Example: Log4Shell (CVE-2021-44228) has a CVSS score of 9.8 and is treated as a Critical alert.

### Scoring Systems
The Common Vulnerability Scoring System (CVSS) is used to measure the severity of vulnerabilities. SOC tools may also use internal risk scoring to help prioritize alerts.

## Key Objective
To develop the ability to assess and prioritize security alerts using standardized criteria to ensure efficient SOC operations.

### References
- FIRST – CVSS framework
- NIST – Incident severity guidance

# 2. Incident Classification
## Core Concepts
### Incident Classification
Incident classification is the process of categorizing security incidents based on their type, behavior, and impact. This helps SOC teams respond consistently and efficiently.
### Incident Categories
- Malware: Malicious software designed to damage or disrupt systems.
- Phishing: Fraudulent emails or messages used to steal credentials or sensitive data.
- DDoS: Attacks that overwhelm systems or networks to cause service disruption.
- Insider Threat: Unauthorized actions performed by trusted users such as employees.
- Data Exfiltration: Unauthorized transfer of sensitive data outside the organization.

### Taxonomy and Frameworks
Standard frameworks are used to label and describe incidents:
- MITRE ATT&CK – Maps attacker tactics and techniques (e.g., T1566 – Phishing).
- ENISA Incident Taxonomy – Provides structured incident classification.
- VERIS Framework – Standard vocabulary for recording and sharing incidents.

### Contextual Metadata
Incidents are enriched with additional details such as:
- Affected systems
- Timestamps
- Source IP addresses
- Indicators of Compromise (IOCs) like malicious IPs, domains, or file hashes

## Key Objective
To build proficiency in categorizing, labeling, and enriching incidents to improve investigation and response efficiency.

# 3. Basic Incident Response
## Core Concepts

### Incident Response Overview
Incident response is the structured approach used by SOC teams to handle security incidents in order to minimize damage and restore normal operations.

### Incident Response Lifecycle
- Preparation: Creating policies, playbooks, and ensuring tools and teams are ready.
- Identification: Detecting and validating security alerts and incidents.
- Containment: Isolating affected systems to prevent further spread.
- Eradication: Removing malware or eliminating the root cause.
- Recovery: Restoring systems and services safely.
- Lessons Learned: Conducting a post-incident review to improve future response.

### Response Procedures
Common incident response actions include:
- Isolating compromised systems
- Preserving digital evidence
- Collecting logs and memory dumps
- Communicating with stakeholders using defined protocols

### Evidence Preservation
Proper evidence handling includes:
- Capturing volatile data such as memory
- Collecting system and security logs
- Hashing files to ensure integrity

## Key Objective
To understand and apply the incident response lifecycle to effectively manage and resolve security incidents.

### References
- NIST SP 800-61 Incident Handling Guide
- SANS Incident Handler’s Handbook
