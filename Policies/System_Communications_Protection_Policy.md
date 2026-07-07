SYSTEM & COMMUNICATIONS PROTECTION POLICY  
Version: 1.0  
Approval Date: 7th July, 2026  
Owner: Information Security Officer (ISO)  
Classification: Internal / Restricted      
________________________________________
1. Purpose  
The purpose of this System & Communications Protection (SCP) Policy is to ensure the confidentiality, integrity, and availability of information transmitted, stored, and processed across Veltrix Pay networks and systems, in accordance with NIST SP 800-53 SC control family and PCI DSS network security requirements.  
________________________________________
2. Scope  
This policy applies to:  
•	All Veltrix Pay information systems  
•	All internal and external network communications, including connections to banks, card networks, and payment processors  
•	All personnel, contractors, and third parties using organizational networks  
•	All technologies enabling system protection (firewalls, encryption, proxies, etc.)  
________________________________________
3. Policy Statements  
3.1 Network Security Controls  
•	Firewalls must be implemented at network boundaries and configured using least privilege.  
•	Network segmentation must be used to isolate sensitive systems, with the cardholder data environment (CDE) segmented from the general corporate network.  
•	Intrusion Detection/Prevention Systems (IDS/IPS) must monitor network traffic.  
3.2 Encryption Requirements  
•	All sensitive data must be encrypted in transit using:  
o	TLS 1.2 or higher  
o	SSH v2  
o	IPSec VPN  
•	Public-facing services must use trusted certificates.  
•	Sensitive data must be encrypted at rest when stored on servers, databases, or backups.  
•	Transaction data transmitted to card networks and banking partners must use end-to-end encryption with key management compliant with PCI DSS Requirement 3 and 4.  
3.3 Boundary Protection  
•	Network boundaries must prevent unauthorized traffic from entering or leaving the network.  
•	All inbound and outbound traffic must be logged.  
•	Unauthorized or suspicious traffic must be blocked and investigated.  
3.4 Secure Communications  
•	Remote access communications must be encrypted (VPN, SSH, TLS).  
•	Management interfaces must not be accessible from the public internet.  
•	Wireless networks must use WPA2-Enterprise or higher security.  
3.5 System Isolation  
•	High-value or sensitive systems must be isolated using:  
o	VLANs  
o	Access Control Lists (ACLs)  
o	Dedicated firewalls  
•	DMZ segments must be used for public-facing applications, including the merchant API gateway.  
3.6 Email & Web Protection  
•	Email must be filtered for malware, spam, and phishing attacks.  
•	Web traffic must be monitored using secure web gateways or proxies.  
•	URL filtering must be enabled to block high-risk sites.  
3.7 Denial-of-Service Protection  
•	Systems must implement protections against DDoS and resource exhaustion attacks.  
•	Critical services, including the payment switch and merchant API, must have redundancy or failover capabilities.  
3.8 Cryptographic Key Management  
•	Encryption keys must be managed according to approved procedures.  
•	Keys must be rotated annually or when compromise is suspected.  
•	Private keys must never be stored in plain text.  
•	Payment encryption keys (PIN block, card data) must be managed using a Hardware Security Module (HSM) per PCI DSS and PCI PIN requirements.  
3.9 Transmission Confidentiality & Integrity  
•	Data integrity checks must be implemented for high-value data transfers.  
•	Sensitive communications must use secure protocols only.  
________________________________________
4. Roles & Responsibilities  
Information Security Officer (ISO)  
•	Maintains this policy  
•	Ensures controls meet NIST, PCI DSS, and organizational requirements  
Network Administrators  
•	Configure firewalls, VPNs, encryption, IDS/IPS  
•	Monitor network activity and enforce segmentations  
System Administrators    
•	Ensure system-level protections (e.g., encryption, ACLs, secure services)  
Users  
•	Must use secure methods when transmitting sensitive data  
•	Must report suspected network or communication issues immediately  
________________________________________
5. Compliance  
Violations of this policy may result in disciplinary action and legal penalties.  
Critical systems must comply with NIST SC controls, PCI DSS network requirements, and Zero Trust Architecture requirements, where applicable.  
________________________________________
6. Review Cycle  
This policy must be reviewed annually or when major system or network changes occur.  
