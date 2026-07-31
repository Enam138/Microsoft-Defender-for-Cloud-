# Microsoft Defender Plans

## Overview

Microsoft Defender for Cloud provides two primary categories of protection:

- **Cloud Security Posture Management (CSPM)**, which continuously assesses Azure resources against security best practices.
- **Cloud Workload Protection (CWP)**, which delivers advanced threat protection for specific Azure workloads such as virtual machines, storage accounts, databases, containers, and Key Vault.

During this project, I reviewed the Defender Plans available for my Azure subscription to understand the security capabilities they provide and determine which plans were appropriate for my environment.


# Objectives

The objectives of this phase were to:

- Review the available Microsoft Defender plans.
- Understand the difference between CSPM and workload protection.
- Evaluate the security capabilities provided by each plan.
- Identify which plans were enabled.
- Assess premium plans that require additional licensing.
- Document future security improvements.


# Defender Plans Dashboard

<img width="1600" height="763" alt="defender plan" src="https://github.com/user-attachments/assets/f95ecaf4-31f6-4e8e-bf57-421ec1796a60" />


# Cloud Security Posture Management (CSPM)

The Defender Plans page showed that **Foundational CSPM** was enabled for the subscription.

Foundational CSPM continuously evaluates Azure resources and provides security recommendations based on Microsoft's Cloud Security Benchmark.

It includes capabilities such as:

- Secure Score
- Security recommendations
- Asset inventory
- Regulatory Compliance
- Security posture assessment

Because Foundational CSPM is included with Microsoft Defender for Cloud, it formed the foundation of this project and enabled continuous visibility into the security posture of my Azure environment.


# Microsoft Defender CSPM

In addition to Foundational CSPM, Microsoft Defender CSPM was also enabled.

Microsoft Defender CSPM extends the foundational capabilities by providing advanced cloud security posture management features such as:

- Attack Path Analysis
- Cloud Security Explorer
- Risk prioritization
- Context-aware security recommendations
- Advanced posture management

During my review, the monitoring coverage was shown as **Partial**, indicating that additional Azure resources could be onboarded to increase visibility.


# Cloud Workload Protection Plans

Microsoft Defender for Cloud also provides workload-specific protection plans for Azure services.

During my assessment, I reviewed the following plans:

| Defender Plan | Status | Purpose |
|---------------|--------|---------|
| Defender for Servers | Off | Protects Azure and hybrid virtual machines |
| Defender for Storage | Off | Detects threats against Azure Storage Accounts |
| Defender for Databases | Off | Protects Azure SQL and other supported databases |
| Defender for App Service | Off | Protects Azure web applications |
| Defender for Containers | Off | Secures AKS and container environments |
| Defender for Key Vault | Off | Monitors Azure Key Vault for suspicious activity |
| Defender for Resource Manager | Off | Detects malicious Azure management operations |


# Why I Did Not Enable Every Defender Plan

One of the most valuable lessons from this project was understanding that security recommendations should be evaluated rather than implemented automatically.

Many Defender workload protection plans require additional licensing and are intended for production environments where advanced threat detection is required.

Since this project focused on Cloud Security Posture Management, enabling every premium Defender plan was outside the scope of the implementation.

Instead, I:

- Reviewed the purpose of each Defender plan.
- Understood the security capabilities provided.
- Evaluated licensing requirements.
- Documented premium plans as future enhancements.

This reflects how cloud security decisions are typically made in enterprise environments, where security improvements must be balanced with business needs, operational requirements, and licensing costs.


# Enterprise Perspective

In a production environment, the selection of Defender plans depends on the organization's workloads.

For example:

- Organizations running virtual machines would typically enable Defender for Servers.
- Businesses hosting customer data in Azure Storage would benefit from Defender for Storage.
- Companies using Azure SQL would often deploy Defender for Databases.
- Enterprises managing secrets and certificates would consider Defender for Key Vault.
- Organizations operating Kubernetes clusters would enable Defender for Containers.

Rather than applying a one-size-fits-all approach, security teams enable only the protections that align with their deployed services and risk profile.


# Key Takeaways

Through this exercise, I gained a better understanding of how Microsoft Defender for Cloud separates security posture management from workload protection.

I also learned that improving cloud security is not simply about enabling every available feature. Instead, effective cloud security requires evaluating business requirements, understanding licensing implications, prioritizing risks, and selecting security controls that provide the greatest value for the environment being protected.


# Skills Demonstrated

- Microsoft Defender for Cloud
- Cloud Security Posture Management (CSPM)
- Microsoft Defender CSPM
- Cloud Workload Protection (CWP)
- Azure Security Governance
- Licensing Awareness
- Security Architecture Evaluation
- Risk-Based Decision Making
- Enterprise Cloud Security Planning

# Conclusion

Reviewing Microsoft Defender Plans helped me understand how organizations tailor cloud security to their specific workloads and operational requirements.

By distinguishing between foundational posture management and advanced workload protection, I developed a broader understanding of Microsoft's cloud security ecosystem and the decision-making process used by cloud security engineers when securing Azure environments.
