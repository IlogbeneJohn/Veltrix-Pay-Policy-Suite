SECURITY ASSESSMENT & AUTHORIZATION POLICY  
Version: 1.0   
Approval Date: 7th july, 2026    
Owner: Information Security Officer (ISO)   
Classification: Internal / Restricted  
________________________________________
1. Purpose  
The purpose of this Security Assessment & Authorization Policy is to define requirements for evaluating security controls, ensuring systems receive appropriate authorization before operating, and maintaining continuous security assurance throughout each system's lifecycle, including annual PCI DSS validation for in-scope systems.  
________________________________________
2. Scope  
This policy applies to:  
•	All Veltrix Pay information systems  
•	All environments hosting organizational data (on-premises, cloud, hybrid)  
•	All employees, contractors, and third-party service providers involved in system development, assessment, or authorization  
•	All components, applications, and services that transmit, store, or process payment or customer information  
________________________________________
3. Policy Statements  
3.1 Security Assessments  
•	Independent security assessments must be conducted before any system is authorized to operate.  
•	Assessments shall evaluate the effectiveness of security controls according to NIST SP 800-53A or approved organizational methodology.  
•	Annual penetration testing and quarterly internal/external vulnerability scans are required for all systems within PCI DSS scope.  
•	Automated assessment tools should be used whenever feasible.  
•	Assessment results must be documented in a Security Assessment Report (SAR).  
________________________________________
3.2 Remediation & Risk Responses  
•	Identified vulnerabilities must be analyzed and assigned risk ratings.  
•	System owners must develop a Plan of Action and Milestones (POA&M) for all unresolved findings.  
•	High-risk findings must be remediated within required timelines as defined by organizational risk tolerance.  
________________________________________
3.3 Authorization to Operate (ATO)  
•	All systems must receive written Authorization to Operate (ATO) from the Authorizing Official (AO) before deployment.  
•	The ATO decision must consider:  
o	Security Assessment Report (SAR) results  
o	POA&M status  
o	Privacy impacts  
o	Residual risk  
o	PCI DSS Attestation of Compliance (AOC) status, where applicable  
•	ATO decisions may result in:  
o	Full Authorization  
o	Interim Authorization (IATT)  
o	Denial of Authorization  
________________________________________
3.4 Continuous Monitoring  
•	Systems must undergo continuous monitoring to ensure ongoing effectiveness of security controls.  
•	Automated monitoring solutions (SIEM, vulnerability scanners, CSPM tools, fraud detection systems) shall be implemented where possible.  
•	Continuous monitoring results must feed into ongoing POA&M updates.  
________________________________________
3.5 Reauthorization Requirements  
•	Systems must be reauthorized at least every 3 years, or sooner if:  
o	Major changes occur  
o	Significant security incidents impact the system  
o	New risks affect system operations  
•	PCI DSS scoped systems require annual reassessment regardless of change activity.  
________________________________________
4. Roles & Responsibilities  
Role	Responsibilities  
Information Security Officer (ISO)	Oversees assessments, ensures compliance with NIST RMF, provides governance.  
Authorizing Official (AO)	Issues ATO decisions and accepts residual risk.  
System Owner	Prepares system documentation, coordinates assessments, manages POA&M.  
Security Control Assessor (SCA)	Performs independent assessments of system controls.  
IT Operations & Engineering Teams	Implement and maintain security controls as required.  
________________________________________
5. Compliance  
Failure to comply with this policy may result in disciplinary action, revocation of access privileges, or other corrective measures as determined by executive leadership.  
________________________________________
6. References    
•	NIST SP 800-37 – Risk Management Framework  
•	NIST SP 800-53A – Security Control Assessments  
•	NIST SP 800-53 – Security and Privacy Controls  
•	PCI DSS v4.0 – Requirements 11 and 12  
•	Organizational Risk Management Strategy  
________________________________________
7. Review & Maintenance  
This policy must be reviewed annually and updated to reflect changes in regulatory requirements, technology environments, or risk posture.  
