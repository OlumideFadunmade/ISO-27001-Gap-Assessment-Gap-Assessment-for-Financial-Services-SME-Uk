# ISO/IEC 27001:2022 Gap Assessment – UK Financial Services SME

## 1.0 Project Overview

This project simulates a **remote ISO/IEC 27001 assessment** conducted for a UK-based financial services SME. The assessment evaluates the organisation’s information security posture, identifies gaps against ISO/IEC 27001 controls, and provides actionable recommendations to improve governance, risk management, and compliance.

## 1.1 Organisation Profile (Simulated)
- **Sector:** Financial Services (UK)
- **Employees:** 75
- **Infrastructure:** Microsoft 365, Azure Cloud, On-premise file server, CRM platform, Financial reporting system
- **Data Processed:** Customer financial records, PII, transaction history, employee HR data
- **Regulatory Context:** UK GDPR, FCA expectations, Data Protection Act 2018

## 2.0 Scope of Assessment
- Evaluate organisation against ISO/IEC 27001:2022 Annex A controls
- Focus on governance, risk management, asset management, access control, incident management, business continuity, and supplier security
- Identify gaps and propose remediation actions

## 2.1 Skills Demonstrated
- ISO/IEC 27001 knowledge and Annex A control mapping
- Risk-based assessment and mitigation planning
- Policy drafting for SME-specific compliance
- Consultancy-style project documentation and reporting

## 2.2 Assessment Methodology

- Asset Identification: Catalogued all critical business assets.

- Threat & Vulnerability Analysis: Identified threats and vulnerabilities for each asset.

- Risk Rating: Calculated Likelihood × Impact (1–5 scale) to assign risk levels (High/Medium/Low).

- Annex A Mapping: Linked each risk to the relevant ISO27001 control.

- Recommendations: Developed a roadmap for remediation and ISO27001 readiness.
 ** The assessment was conducted remotely, including documentation review, stakeholder interviews, and system inspections.**

## 3.0 Risk Register

| Risk ID | Asset                   | Threat              | Vulnerability              | Likelihood | Impact | Risk Rating | Risk Level | Existing Controls | Mitigation Actions                   | Owner              |
| ------- | ----------------------- | ------------------- | -------------------------- | ---------- | ------ | ----------- | ---------- | ----------------- | ------------------------------------ | ------------------ |
| R001    | Customer Financial DB   | Unauthorized Access | No MFA                     | 4          | 5      | 20          | High       | User passwords    | Implement MFA; quarterly review      | IT Manager         |
| R002    | CRM Platform            | Data Loss           | No Backup                  | 3          | 4      | 12          | Medium     | Manual backup     | Automated cloud backup               | IT Manager         |
| R003    | Microsoft 365           | Account Compromise  | Weak Password              | 3          | 5      | 15          | Medium     | Password policy   | Enforce strong passwords & MFA       | IT Manager         |
| R004    | Financial Reporting Sys | Data Corruption     | No validation              | 3          | 4      | 12          | Medium     | Manual checks     | Automated validation                 | Finance Manager    |
| R005    | Employee Laptops        | Malware             | Outdated AV                | 4          | 4      | 16          | High       | Antivirus         | Update AV daily; endpoint monitoring | IT Manager         |
| R006    | File Server             | Unauthorized Access | Weak permissions           | 3          | 5      | 15          | Medium     | ACLs              | Review permissions quarterly         | IT Manager         |
| R007    | CRM Platform            | Insider Threat      | No monitoring              | 2          | 5      | 10          | Medium     | Audit logs        | Implement real-time monitoring       | Compliance Officer |
| R008    | Customer Financial DB   | Ransomware          | No offline backup          | 4          | 5      | 20          | High       | Cloud backup      | Offline encrypted backup             | IT Manager         |
| R009    | Employee Laptops        | Lost Device         | No encryption              | 3          | 4      | 12          | Medium     | Disk encryption   | Full disk encryption; remote wipe    | IT Manager         |
| R010    | Microsoft 365           | Phishing            | No training                | 3          | 4      | 12          | Medium     | Email filters     | Phishing awareness training          | IT Manager         |
| R011    | Financial Reporting Sys | Compliance Failure  | Missing policy             | 2          | 5      | 10          | Medium     | Existing SOPs     | Implement formal policies            | Compliance Officer |
| R012    | File Server             | Hardware Failure    | No redundancy              | 3          | 3      | 9           | Medium     | Daily backup      | Implement RAID / redundancy          | IT Manager         |
| R013    | CRM Platform            | Data Leakage        | Third-party access         | 3          | 4      | 12          | Medium     | Contracts         | Supplier NDAs & access review        | Compliance Officer |
| R014    | Customer Financial DB   | Insider Threat      | Privileged misuse          | 3          | 5      | 15          | Medium     | Audit logs        | Monitor privileged users             | IT Manager         |
| R015    | Employee Laptops        | Unpatched OS        | Vulnerability exploitation | 4          | 4      | 16          | High       | Patch management  | Automate OS patching                 | IT Manager         |

Likelihood (1-5),  Impact (1-5),  Risk Rating (Likelihood x Impact, formula included),  Risk Level (High/Medium/Low, formula included) 

## 4.0 Gap Assessment Findings
| Area                | Observation                          | Gap / Risk                      | Risk Level | Recommendation                                         |
| ------------------- | ------------------------------------ | ------------------------------- | ---------- | ------------------------------------------------------ |
| Governance          | Roles defined but not communicated   | Partial governance framework    | Medium     | Communicate roles; assign security responsibilities    |
| Risk Management     | Risk register exists but not updated | Informal process                | High       | Formalise risk assessment and periodic review          |
| Access Control      | Privileged accounts not reviewed     | Weak access management          | High       | Implement JML, MFA, and quarterly review               |
| Incident Management | No formal incident response SLA      | Unprepared for breaches         | High       | Develop and test Cyber Security Incident Response Plan |
| Supplier Security   | Contracts lack security clauses      | Third-party risk                | Medium     | Implement supplier assessments and NDAs                |
| Business Continuity | Backup strategy exists but untested  | Recovery objectives undefined   | Medium     | Test backup and recovery, define RTO/RPO               |
| Asset Management    | Assets tracked but not classified    | Missing criticality & ownership | Medium     | Create formal asset register and classification        |
| Security Awareness  | Staff training irregular             | Low awareness                   | Medium     | Conduct mandatory ISO27001-aligned training            |

**Total Risks Identified: 15 (High: 5, Medium: 7, Low: 3)**

## 5.0 Annex A Mapping

| Control ID | Control Name             | Objective                  | Current Status  | Gap Description                  | Risk IDs Linked | Remediation Action              | Owner              |
| ---------- | ------------------------ | -------------------------- | --------------- | -------------------------------- | --------------- | ------------------------------- | ------------------ |
| A.5.1      | Info Sec Policies        | Provide direction          | Partial         | Policy not communicated          | R011            | Communicate and train staff     | Compliance Officer |
| A.6.1      | Org of Info Security     | Assign responsibilities    | Not Implemented | No defined roles                 | R001,R007       | Define roles & responsibilities | IT Manager         |
| A.8.1      | Asset Management         | Identify & classify assets | Partial         | Assets unclassified              | R001,R002,R006  | Create asset register           | IT Manager         |
| A.9.1      | Access Control           | Control access             | Partial         | Privileged accounts not reviewed | R001,R006,R014  | Enforce JML & MFA               | IT Manager         |
| A.12.6     | Vulnerability Management | Manage vulnerabilities     | Partial         | Laptops unpatched                | R015            | Automate patch management       | IT Manager         |
| A.16.1     | Incident Management      | Respond to incidents       | Partial         | Incident plan untested           | R003,R008       | Test incident response plan     | IT Manager         |

 
# 6.0 Information Security Policy – Financial Services SME

## 6.1  Purpose
Protect confidentiality, integrity, and availability of financial and personal data.

## 6.2 Scope
Applies to all employees, contractors, and IT systems.

## 6.3 Key Policies
- **Access control:** Unique user IDs, MFA, least privilege, quarterly review
- **Risk management:** Annual assessment, documented risk register
- **Incident management:** Report within 24h; ICO notification within 72h
- **Supplier security**: Due diligence, DPAs, annual review
- **Business continuity**: Daily backups, defined RTO/RPO, annual test
- **Compliance:** Aligns with ISO 27001, UK GDPR, FCA guidance

# 7.0 Recommendations & Roadmap (12 months)

## Short-term (0-3 Months)
- Formalise ISMS governance and communicate roles
- Update risk register and implement periodic review
- Implement MFA and access review procedures

## Medium-term (3-6 Months)
- Conduct internal audit against ISO27001 Annex A controls
- Develop and test Cyber Security Incident Response Plan (CSIRP)
- Enforce supplier assessments and NDAs

## Long-term (6-12 Months)
- Review business continuity and recovery objectives
- Conduct ISO27001 Stage 1 readiness review
- Finalise all policies and training programs
  ---
# 8.0 Executive Summary
- Remote ISO/IEC 27001 assessment identified gaps in governance, risk management, access control, supplier security, and business continuity. Recommendations focus on implementing formal ISMS practices and preparing the SME for ISO 27001 certification.
