CONFIGURATION MANAGEMENT POLICY  
Version: 1.0  
Approval Date: 7th July, 2026  
Owner: Information Security Officer (ISO)  
Classification: Internal / Restricted  
________________________________________
1. Purpose  
The purpose of this Configuration Management Policy is to establish requirements for managing configuration changes, maintaining secure baselines, and ensuring that Veltrix Pay's payment processing systems remain in a known, trusted state.  
________________________________________
2. Scope  
This policy applies to:  
•	All Veltrix Pay information systems  
•	All software, hardware, applications, and cloud resources, including the payment switch, ledger, and API gateway  
•	All employees, contractors, and administrators who manage system configurations  
________________________________________  
3. Policy Statements  
3.1 Configuration Baselines  
•	All systems must have an approved security configuration baseline.    
•	Baselines must comply with industry standards (e.g., CIS Benchmarks, DISA STIGs) and PCI DSS hardening requirements.  
•	Baselines must be reviewed annually and updated as necessary.  
3.2 Change Management  
•	All configuration changes must follow the organization's Formal Change Control Process.  
•	Changes to production payment processing systems require dual approval from Engineering and the ISO.  
•	Emergency changes must be documented within 24 hours and reviewed at the next CAB meeting.  
•	Unauthorized or undocumented changes are strictly prohibited.  
3.3 Configuration Documentation  
•	System configurations must be documented and kept up to date.  
•	Diagrams, inventories, and configuration files must be stored securely.  
•	Cloud resource configurations must be captured via IaC (Infrastructure as Code) where possible.  
3.4 Access Restrictions for Changes  
•	Only authorized administrators may modify system configurations.  
•	Privileged accounts must be used only when needed to perform configuration tasks.  
•	Multi-factor authentication must be used for all administrative access.  
3.5 Monitoring & Detection of Unauthorized Changes  
•	Systems must be monitored to detect unauthorized or unexpected configuration changes.  
•	File Integrity Monitoring (FIM) tools must be used for high-value systems, including the ledger database and payment switch.  
•	All detected unauthorized changes must trigger an incident response.  
3.6 Patch & Update Management  
•	Security patches must be applied within:  
o	24 hours for critical vulnerabilities  
o	7 days for high vulnerabilities  
o	30 days for medium vulnerabilities  
•	All patches must be tested before deployment except during emergencies.  
•	Unsupported software is prohibited in production environments.  
3.7 Configuration Backups  
•	System configuration files must be backed up regularly and stored securely.  
•	Backups must be encrypted and tested quarterly for restoration capability.  
________________________________________
4. Roles & Responsibilities  
Information Security Officer (ISO)  
•	Maintains this policy and ensures compliance.  
•	Approves configuration baselines.  
Change Advisory Board (CAB)  
•	Reviews and approves requested changes.  
•	Assesses risks, impacts, and rollback plans.  
System Administrators  
•	Implement approved changes.  
•	Maintain configuration documentation and apply patches timely.  
________________________________________
5. Compliance  
Non-compliance may result in disciplinary action and possible legal or regulatory consequences.  
________________________________________
6. Review Cycle  
This policy must be reviewed annually or upon significant system changes.  
