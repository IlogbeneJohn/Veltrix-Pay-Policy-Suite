IDENTIFICATION & AUTHENTICATION POLICY  
Version: 1.0  
Approval Date: 7th July, 2026
Owner: Information Security Officer (ISO)  
Classification: Internal / Restricted  
________________________________________
1. Purpose  
The purpose of this Identification & Authentication (IA) Policy is to ensure that all users, devices, and systems accessing Veltrix Pay resources are uniquely identified, authenticated, and authorized in accordance with NIST SP 800-53 IA control family, NIST SP 800-63 Digital Identity Guidelines, and PCI DSS authentication requirements.  
________________________________________
2. Scope  
This policy applies to:  
•	All information systems and applications  
•	All employees, contractors, and third-party users  
•	All authentication mechanisms (passwords, MFA, certificates, tokens)  
•	All devices connecting to Veltrix Pay networks  
________________________________________
3. Policy Statements  
3.1 Unique Identification  
•	Each user must be assigned a unique user ID.  
•	Shared, generic, or group accounts are prohibited unless explicitly approved by the ISO.  
•	System-level accounts (e.g., service accounts) must follow documented naming conventions.  
3.2 Authentication Requirements  
•	All users must authenticate using approved methods before accessing any system.  
•	Multi-Factor Authentication (MFA) is required for:  
o	All privileged accounts  
o	Remote access  
o	Cloud-based accounts  
o	VPN access  
o	All access to the cardholder data environment (CDE)  
•	Authentication mechanisms must follow NIST 800-63B standards.  
•	Customer-facing authentication for fund transfers above defined thresholds must require step-up authentication (OTP or biometric).  
3.3 Password Standards  
All passwords must comply with the following minimum requirements:  
•	Minimum length: 14 characters  
•	Must contain a mix of uppercase, lowercase, numbers, and symbols  
•	Must not contain usernames or easily guessable patterns  
•	Passwords must be changed at least every 90 days  
•	Password reuse: last 10 passwords cannot be reused  
If system uses NIST modern password guidance, then:  
•	Length-based password policies apply  
•	No forced rotation unless compromised  
3.4 Device Identification  
•	All systems must authenticate devices before granting network access.  
•	Certificates, MDM enrollment, or domain join are required for trusted devices.  
•	Mobile devices used to access the merchant dashboard must be enrolled in MDM.  
3.5 Service & System Account Controls  
•	Service accounts must not be used by people.  
•	Passwords and API keys for service accounts must be stored securely (vault).  
•	Service accounts must be reviewed quarterly.  
•	API keys issued to merchant integrations must be scoped to least-privilege endpoints only.  
3.6 Failed Login Attempts  
•	User accounts must lock after 5 failed attempts.  
•	Automatic lockout duration: 15 minutes, or manual unlock by admin.  
•	Repeated failed attempts must trigger alerting and review.  
•	Customer accounts must lock after 5 failed login attempts and require identity re-verification to unlock.  
3.7 Session Management  
•	Sessions must automatically log out after 15 minutes of inactivity.  
•	Remote sessions must use encrypted protocols only (SSH, HTTPS, VPN).  
•	Session tokens must be protected from reuse and hijacking.  
3.8 Cryptographic Requirements  
•	Passwords must be hashed using strong algorithms (e.g., bcrypt, PBKDF2, Argon2).  
•	Authentication data must not be transmitted in clear text.  
•	Cardholder authentication data must never be stored after transaction authorization, per PCI DSS Requirement 3.  
________________________________________
4. Roles & Responsibilities  
Information Security Officer (ISO)  
•	Maintains this policy  
•	Ensures MFA, password, and identity controls meet standards  
System Administrators  
•	Implement identity and authentication mechanisms  
•	Maintain identity systems such as Active Directory, SSO, or MFA systems  
Users  
•	Maintain password confidentiality  
•	Report authentication issues or suspicious activity immediately  
________________________________________
5. Compliance  
Non-compliance may result in disciplinary action, revocation of access, and increased monitoring.  
Regulated systems must comply with NIST SP 800-53 IA controls, PCI DSS, and related audit requirements.  
________________________________________
6. Review Cycle  
This policy must be reviewed annually or upon major changes in authentication technologies or organizational requirements.  
