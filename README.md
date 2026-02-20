# Governance-Risk-and-Compliance-GRC-Security-Assessment
Enterprise GRC security assessment aligned to NIST 800-53 and PCI DSS, including risk analysis, control evaluation, and a phased remediation roadmap.
**ABC Corporation – Enterprise Risk & Compliance Evaluation**  
Isabel Romero | M.S. Cybersecurity  

---

## Executive Summary

This assessment evaluates the security posture of ABC Corporation’s enterprise IT environment. The review identified critical gaps in access control, authentication, endpoint protection, risk governance, and PCI DSS compliance.

Controls were evaluated against NIST SP 800-53, NIST SP 800-30, OMB Circular A-130, and PCI DSS v4.0. Based on identified deficiencies, a prioritized remediation roadmap was developed to reduce regulatory exposure, strengthen governance maturity, and improve operational security.

> **Note:** ABC Corporation is a fictional organization used for portfolio demonstration purposes.

---

# Security Control Gap Analysis

A review of the current environment identified the following high-impact deficiencies:

## 1. Access Control Weaknesses
- No formal least privilege enforcement
- User permissions not aligned to job roles
- No structured access recertification process
- Increased risk of insider misuse and lateral movement

## 2. Legacy Infrastructure
- End-of-life firewall in production
- Unsupported systems increase exposure to known vulnerabilities
- Limited defensive capability against modern threats

## 3. Weak Authentication Controls
- No multi-factor authentication (MFA)
- Elevated risk of credential compromise
- Sensitive systems accessible via single-factor authentication

## 4. Endpoint Protection Gaps
- Inconsistent antivirus deployment
- No centralized monitoring of endpoints
- Increased ransomware and malware exposure risk

## 5. PCI DSS Compliance Gaps
- No proper POS network segmentation
- Firewall configuration deficiencies
- Inadequate endpoint controls for payment systems

## 6. Governance Deficiencies
- No recurring enterprise risk assessment
- No documented risk response framework
- No formal Information Security Program Plan (ISPP)
- No centralized POA&M tracking

**Overall Assessment:**  
The organization demonstrates reactive security practices with limited governance maturity. Immediate remediation is required to reduce regulatory and operational risk.

---

# Control Risk Analysis

| Control  | Description           | Risk Level | Business Impact                                 |
|----------|-----------------------|------------|-------------------------------------------------|
| AC-6     | Least Privilege       | High       | Unauthorized access to PHI and critical systems |
| CA-7     | Continuous Monitoring | High       | Undetected threats and prolonged dwell time     |
| RA-3     | Risk Assessment       | High       | Lack of visibility into enterprise risk posture |
| CA-5     | POA&M                 | Moderate   | Delayed remediation and audit findings          |
| RA-7     | Risk Response         | Moderate   | Inconsistent risk treatment decisions           |

---

## Example Control Breakdown

### AC-6 — Least Privilege (High Risk)

**Issue:** Excessive permissions and no formal access review process.  
**Impact:** Increased likelihood of insider threat, credential abuse, and data compromise.  
**Remediation Approach:** Implement role-based access control (RBAC) and periodic access recertification.

---

# Risk-Based Remediation Roadmap

Remediation actions were prioritized based on risk severity and compliance exposure.

---

## Phase 1: Immediate (0–30 Days)

### Implement Least Privilege (AC-6)
- Deploy RBAC aligned to job functions
- Remove excessive permissions
- Enforce quarterly access reviews  
**Owner:** IAM Team

### Deploy Continuous Monitoring (CA-7)
- Implement SIEM (e.g., Splunk or Microsoft Sentinel)
- Centralize log aggregation
- Establish alert thresholds  
**Owner:** Security Operations

---

## Phase 2: Governance Strengthening (30–90 Days)

### Conduct Enterprise Risk Assessment (RA-3)
- Perform risk analysis aligned to NIST SP 800-30
- Document threats, vulnerabilities, likelihood, and impact
- Present findings to executive leadership  
**Owner:** GRC Team

### Formalize Risk Response (RA-7)
- Define risk tolerance thresholds
- Implement risk response matrix
- Require executive risk acceptance sign-off  
**Owner:** CISO / Risk Committee

### Implement POA&M Tracking (CA-5)
- Deploy centralized remediation tracking system
- Assign accountability and deadlines
- Conduct monthly progress reviews  
**Owner:** GRC Team

---

# PCI DSS–Aligned POS Security Policy

## Purpose
Establish minimum security controls for protecting cardholder data and ensuring PCI DSS v4.0 compliance.

---

## Key Requirements

### Network Security (PCI Requirement 1)
- Next-generation firewall required
- POS network segmentation enforced
- Deny-by-default firewall posture
- Biannual firewall rule review

### Anti-Malware (PCI Requirement 5)
- Centrally managed endpoint protection
- Automated signature updates
- Weekly system scans
- SIEM integration for alerting

### Secure Configuration (PCI Requirement 2)
- Remove vendor default credentials
- Disable unused services and ports
- Enforce strong password policies
- Unique administrative credentials required

---

## Monitoring & Validation
- POS systems included in centralized logging
- Quarterly internal vulnerability scans
- Annual PCI DSS compliance validation

---

# Framework Alignment

- NIST SP 800-53 Rev 5  
- NIST SP 800-30  
- OMB Circular A-130  
- PCI DSS v4.0  

---

# Key Outcomes

- Reduced excessive privilege exposure
- Improved threat detection capability
- Established structured enterprise risk governance
- Strengthened PCI DSS compliance posture
- Increased executive visibility into organizational risk

---
