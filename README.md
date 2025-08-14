# CST8919 – DevOps Security and Compliance

# Cloud Security & Compliance Service Comparison

## Objective

This document compares the **Microsoft Azure** security and compliance services used in the "Security and Compliance" course with their **Amazon Web Services (AWS)** and **Google Cloud Platform (GCP)** equivalents.  
It includes a high-level comparison table and a detailed breakdown of features, security/compliance capabilities, pricing, and integration with DevSecOps practices.

---

## Quick Comparison Table

| Azure Service | AWS Equivalent | GCP Equivalent |
|---------------|---------------|----------------|
| Azure Active Directory (SSO, IAM) | AWS IAM & AWS SSO | Cloud Identity & IAM |
| Azure Monitor & Log Analytics | Amazon CloudWatch | Google Cloud Operations Suite (formerly Stackdriver) |
| Azure Policy | AWS Organizations & AWS Config | Google Cloud Organization Policy Service |
| Defender for Cloud | AWS Security Hub | Security Command Center |
| Azure Sentinel (SIEM/SOAR) | Amazon Security Lake & Amazon GuardDuty (partial SIEM) | Chronicle Security Operations |

---

## Detailed Comparisons

### 1. Azure Active Directory (SSO, IAM)

**Overview**  
- **Azure AD**: Cloud-based identity and access management, enabling SSO, MFA, and conditional access.

**AWS Equivalent – IAM & AWS SSO**  
- IAM manages users, roles, and permissions.  
- AWS SSO provides SSO across AWS accounts and third-party applications.

**GCP Equivalent – Cloud Identity & IAM**  
- Cloud Identity handles user lifecycle, SSO, and MFA.  
- GCP IAM controls permissions at resource and project levels.

**Core Features**
- **Azure AD**: Enterprise app SSO, conditional access policies, hybrid identity.  
- **AWS**: Fine-grained permissions, federated access, integrated SSO.  
- **GCP**: Context-aware access, unified identity for GCP and Google Workspace.

**Security & Compliance**
- Azure AD: ISO 27001, SOC, FedRAMP, HIPAA.  
- AWS IAM/SSO: SOC, ISO 27001, FedRAMP.  
- GCP: ISO 27001, FedRAMP, HIPAA, GDPR.

**Pricing Model**
- Azure AD: Free tier + Premium P1/P2 licensing.  
- AWS IAM: No additional cost; SSO based on user/month pricing.  
- GCP Cloud Identity: Free & Premium editions.

**Integration for DevSecOps**
- All integrate with CI/CD pipelines, automation scripts, and security tools.

---

### 2. Azure Monitor & Log Analytics

**Overview**  
- **Azure Monitor**: Metrics & logs for applications and infrastructure.  
- **Log Analytics**: Advanced querying and visualization for logs.

**AWS Equivalent – Amazon CloudWatch**  
- Metrics, logs, events, alarms, and dashboards for AWS resources.

**GCP Equivalent – Cloud Operations Suite**  
- Includes Monitoring, Logging, Trace, Error Reporting, and Profiling.

**Core Features**
- Azure: Kusto Query Language (KQL), cross-resource analytics.  
- AWS: Metrics filters, anomaly detection, composite alarms.  
- GCP: Integration with BigQuery, log-based metrics, custom dashboards.

**Security & Compliance**
- All major certifications: ISO, SOC, HIPAA, FedRAMP.

**Pricing Model**
- Based on data ingestion, retention, and API calls.

**Integration for DevSecOps**
- All integrate with automation tools like Terraform, CI/CD workflows.

---

### 3. Azure Policy

**Overview**  
- **Azure Policy**: Enforce organization-specific rules for resource configurations.

**AWS Equivalent – AWS Organizations & AWS Config**  
- AWS Organizations manages accounts, policies, and service control policies.  
- AWS Config enforces compliance and monitors configuration changes.

**GCP Equivalent – Organization Policy Service**  
- Defines and enforces constraints across projects/folders.

**Core Features**
- Azure: Initiative definitions, compliance dashboard.  
- AWS: SCPs, config rules, drift detection.  
- GCP: Resource constraints, centralized policy management.

**Security & Compliance**
- All support compliance standards like PCI-DSS, HIPAA, ISO.

**Pricing Model**
- Azure Policy: Free, charges may apply for remediation tasks.  
- AWS Config: Pay per configuration item.  
- GCP: Included in platform usage.

**Integration for DevSecOps**
- All support automated compliance checks in CI/CD.

---

### 4. Defender for Cloud

**Overview**  
- **Defender for Cloud**: Unified security management and threat protection.

**AWS Equivalent – AWS Security Hub**  
- Centralized view of security alerts and compliance status.

**GCP Equivalent – Security Command Center**  
- Asset discovery, vulnerability scanning, threat detection.

**Core Features**
- Azure: Threat protection, regulatory compliance dashboard.  
- AWS: Aggregates findings from GuardDuty, Inspector, Macie.  
- GCP: Tiered security services (Standard & Premium).

**Security & Compliance**
- All integrate with compliance frameworks (CIS, NIST, PCI-DSS).

**Pricing Model**
- Defender for Cloud: Tier-based per resource type.  
- AWS Security Hub: Per finding ingested.  
- GCP SCC: Premium tier per asset scanned.

**Integration for DevSecOps**
- All integrate with alerting, automation, and security orchestration.

---

### 5. Azure Sentinel (SIEM/SOAR)

**Overview**  
- **Azure Sentinel**: Cloud-native SIEM with SOAR capabilities.

**AWS Equivalent – Amazon Security Lake & GuardDuty**  
- Security Lake centralizes security data; GuardDuty detects threats (partial SIEM functionality).

**GCP Equivalent – Chronicle Security Operations**  
- SIEM and SOAR platform for log ingestion, correlation, and threat hunting.

**Core Features**
- Azure: AI-driven threat detection, playbooks with Logic Apps.  
- AWS: Central log storage, anomaly detection, partner integrations.  
- GCP: Threat intelligence, detection rules, integrated automation.

**Security & Compliance**
- Meets global security standards; integrates with compliance tooling.

**Pricing Model**
- Azure Sentinel: Pay-as-you-go per GB ingested.  
- AWS: Storage and query costs for Security Lake, GuardDuty per event.  
- GCP Chronicle: Subscription or usage-based.

**Integration for DevSecOps**
- Supports automated incident response, pipeline security alerts.

---

## Summary

All three cloud providers offer equivalent services for identity management, monitoring, policy enforcement, security posture management, and SIEM/SOAR capabilities. While features overlap significantly, differences emerge in **pricing models**, **native integrations**, and **tooling maturity**.  
Choosing between them often comes down to existing ecosystem investments and specific compliance requirements.
