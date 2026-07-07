AUDIT & ACCOUNTABILITY POLICY  
Version: 1.0  
Approval Date: 7th, July 2026.  
Owner: Information Security Officer (ISO)  
Classification: Internal / Restricted  
________________________________________
1. Purpose  
The purpose of this Audit & Accountability Policy is to ensure that Veltrix Pay collects, analyzes, and retains audit logs necessary to support security investigations, incident response, fraud detection, and compliance with applicable regulatory and internal requirements, including PCI DSS and Central Bank of Nigeria (CBN) guidelines.  
________________________________________
2. Scope  
This policy applies to:  
•	All Veltrix Pay information systems  
•	All employees, contractors, and third parties  
•	All systems, devices, and applications that store, transmit, or process payment or customer data  
________________________________________
3. Policy Statements  
3.1 Audit Log Generation  
•	All systems must generate audit logs for security-relevant events.  
•	Logs must include sufficient detail to identify who, what, when, and where an event occurred.  
•	Systems must be configured to log authentication events, privilege use, configuration changes, and administrative actions.  
•	All transactions processed through the payment switch must generate an immutable audit trail.  
3.2 Log Protection  
•	Audit logs must be protected from unauthorized access, modification, and deletion.  
•	Only authorized personnel may access or manage audit log storage systems.  
•	Logs must be digitally signed or checksum-protected where feasible.  
3.3 Log Retention  
•	Audit logs must be retained for a minimum of 90 days online and 1 year archived, unless otherwise mandated by regulation.  
•	Transaction and ledger logs must be retained for a minimum of 7 years per CBN and tax recordkeeping requirements.  
•	Archived logs must be encrypted at rest and stored securely.  
3.4 Log Review & Monitoring  
•	Security logs must be reviewed daily by the security team or SIEM automation.  
•	Suspicious or anomalous activity must be investigated promptly.  
•	High-risk alerts must be escalated to the ISO or Incident Response Team.  
•	Transaction monitoring rules must flag unusual transfer volumes, velocity, or geographic anomalies for fraud review.  
3.5 Time Synchronization  
•	All systems must synchronize to an approved NTP time source.  
•	Time drift greater than ±2 minutes must be corrected immediately.  
3.6 Administrator & Privileged User Monitoring  
•	All privileged user activities must be logged and monitored.   
•	Administrative sessions should be captured using session recording tools when applicable.  
•	Direct database access to the ledger system must be logged at the query level.  
3.7 Log Failures  
•	Systems must generate alerts when logging functions fail, log storage is full, or logs cannot be transmitted.  
•	Systems with disabled or broken logging must be removed from production until corrected.  
________________________________________
4. Roles & Responsibilities  
Information Security Officer (ISO)  
•	Owns and maintains this policy.  
•	Ensures audit controls meet regulatory requirements.  
System Administrators  
•	Configure systems to generate required logs.  
•	Ensure logs are transmitted to centralized logging infrastructure.  
Security Operations Team (SOC)  
•	Reviews logs and investigates alerts.  
•	Maintains SIEM rules, alerts, and dashboards.  
Fraud & Risk Team  
•	Reviews transaction logs for indicators of fraud.  
•	Coordinates with SOC on suspicious activity escalations.  
________________________________________
5. Compliance  
Failure to comply with this policy may result in disciplinary action, up to and including termination, and may expose Veltrix Pay to legal and regulatory penalties.  
________________________________________
6. Review Cycle  
This policy must be reviewed annually or whenever significant changes occur in technology, regulations, or business operations.  
