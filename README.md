# Microsoft Defender for Cloud – Cloud Security Posture Management

![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Microsoft Defender](https://img.shields.io/badge/Microsoft%20Defender-5E5E5E?style=for-the-badge&logo=microsoft&logoColor=white)
![Azure Monitor](https://img.shields.io/badge/Azure%20Monitor-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Log Analytics](https://img.shields.io/badge/Log%20Analytics-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Cloud Security](https://img.shields.io/badge/Cloud%20Security-Implemented-success?style=for-the-badge)

![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Microsoft%20Azure-blue?style=flat-square)


## Project Overview

## Project Overview

This project demonstrates how I used Microsoft Defender for Cloud to assess, monitor, and improve the security posture of an Azure environment.

Rather than deploying a new environment solely for this project, I built on the secure Azure infrastructure created in my previous Azure Security project. This allowed me to evaluate an existing cloud environment using Microsoft Defender for Cloud and gain practical experience with Cloud Security Posture Management (CSPM), Secure Score, Regulatory Compliance, security recommendations, centralized monitoring, and governance.

Throughout the project, I approached Microsoft Defender for Cloud from the perspective of a Cloud Security Engineer. Instead of simply enabling every available recommendation, I evaluated each recommendation, assessed its business impact, considered licensing requirements, implemented appropriate security improvements, and documented recommendations that required additional services or premium licensing.


## Business Scenario

Contoso Health Services has migrated several workloads to Microsoft Azure. As cloud adoption increased, the organization required continuous visibility into the security posture of its Azure resources.

As the Cloud Security Engineer responsible for securing the Azure environment, I implemented Microsoft Defender for Cloud to:

- Continuously assess Azure resources.
- Improve cloud security posture.
- Review security recommendations.
- Monitor Secure Score.
- Evaluate Regulatory Compliance.
- Strengthen monitoring and auditing.
- Improve governance across Azure resources.

The objective was to improve visibility into cloud security while following Microsoft's security best practices and Zero Trust principles.

# Project Objectives

During this project I implemented and evaluated:

- Microsoft Defender for Cloud
- Cloud Security Posture Management (CSPM)
- Azure Secure Score
- Microsoft Cloud Security Benchmark
- Regulatory Compliance
- Security Recommendations
- Azure Key Vault Diagnostic Logging
- Azure Monitor
- Log Analytics Workspace
- Email Notifications
- Azure Resource Security Validation


# Azure Services Used

| Service | Purpose |
|----------|---------|
| Microsoft Defender for Cloud | Cloud Security Posture Management |
| Azure Key Vault | Secrets management |
| Azure Monitor | Monitoring and diagnostics |
| Log Analytics Workspace | Centralized log collection |
| Azure Storage Account | Secure storage |
| Azure Virtual Network | Secure networking |
| Network Security Groups | Traffic filtering |
| Microsoft Entra ID | Identity and access management |
| Azure RBAC | Authorization |


# Architecture

<img width="1672" height="941" alt="ChatGPT Image Jul 30, 2026, 02_53_10 AM" src="https://github.com/user-attachments/assets/5ec0fef1-5a4a-4340-b320-1ff013207dba" />


The architecture illustrates how Microsoft Defender for Cloud continuously assesses Azure resources, evaluates compliance, generates security recommendations, and integrates with Azure Monitor and Log Analytics to improve visibility into cloud security events.

Additional architecture details are available in **Architecture.md**.

# Features Implemented

## Security Posture Management

- Microsoft Defender for Cloud
- Foundational CSPM
- Microsoft Defender CSPM
- Secure Score Analysis
- Security Recommendations

## Monitoring

- Email Notifications
- Log Analytics Workspace
- Azure Monitor
- Azure Key Vault Diagnostic Logs
- Centralized Logging

## Governance

- Regulatory Compliance
- Microsoft Cloud Security Benchmark
- Subscription Owner Validation
- Azure RBAC Review

## Resource Security

- Azure Key Vault
- Azure Storage Account
- Azure Networking
- Identity Security Validation


# Project Walkthrough

## Step 1 — Reviewed Microsoft Defender for Cloud

I explored the Defender for Cloud dashboard to understand the current security posture of my Azure environment.

**Screenshot**

<img width="1600" height="760" alt="defender for cloud overview" src="https://github.com/user-attachments/assets/a2723eaa-a3fe-4cc1-8137-07dc7109d56b" />


## Step 2 — Reviewed Secure Score

I analyzed Secure Score to understand the overall security health of my Azure subscription and prioritize recommendations.

<img width="1600" height="761" alt="security posture" src="https://github.com/user-attachments/assets/7d7367d9-55a4-4b8b-958e-8df1b84cbb2d" />


## Step 3 — Investigated Security Recommendations

I reviewed each recommendation, determined whether it could be implemented within my environment, and documented licensing-dependent recommendations separately.

<img width="1600" height="760" alt="recommendation" src="https://github.com/user-attachments/assets/068f14cf-8b9a-4e1f-b512-0dbb248e65ab" />


## Step 4 — Configured Email Notifications

I configured Microsoft Defender for Cloud email notifications to improve operational awareness and ensure that high-severity security alerts would be delivered to designated recipients.

<img width="1600" height="756" alt="email notify" src="https://github.com/user-attachments/assets/40aff8af-b811-4e7c-b142-230eb69ac587" />


## Step 5 — Implemented Centralized Logging

To improve monitoring and auditing, I created a Log Analytics Workspace and configured Azure Key Vault diagnostic logging.

### Log Analytics Workspace

<img width="941" height="905" alt="log ana work" src="https://github.com/user-attachments/assets/47418770-c430-439d-8088-ec89458f1bef" />


### Key Vault Diagnostic Settings

<img width="942" height="910" alt="key vault diag" src="https://github.com/user-attachments/assets/8bb5acde-99d2-4c57-afcc-022dbc77df4d" />


## Step 6 — Evaluated Regulatory Compliance

I reviewed the Microsoft Cloud Security Benchmark and analyzed multiple security control families, including Network Security, Identity Management, Data Protection, Logging, and Incident Response.

### Regulatory Dashboard

<img width="1600" height="765" alt="compliance" src="https://github.com/user-attachments/assets/f0d51cb9-d887-4512-9570-a95eff263c49" />


# Skills Demonstrated

Through this project I demonstrated practical experience with:

- Microsoft Defender for Cloud
- Cloud Security Posture Management
- Azure Governance
- Secure Score Analysis
- Regulatory Compliance
- Azure Monitoring
- Log Analytics
- Azure Key Vault Security
- Azure RBAC
- Security Recommendations
- Risk Assessment
- Security Validation
- Cloud Security Operations

# Key Takeaways

This project reinforced that cloud security extends beyond deploying secure infrastructure. I learned how to continuously assess cloud resources, prioritize security recommendations, improve monitoring, validate configurations, and evaluate compliance using Microsoft Defender for Cloud.

One of the most valuable lessons was understanding that security recommendations should be assessed within the context of business requirements, architecture, licensing, and operational impact rather than implemented indiscriminately.

# Related Projects

- Azure Secure Infrastructure
- Microsoft Entra ID Identity Security
- Microsoft Defender for Cloud Security Posture Management

Together, these projects demonstrate practical experience across infrastructure security, identity security, governance, monitoring, and cloud security operations.

# Author

**Sampson Manyo**

Cloud Security Engineer | Cybersecurity Analyst | Azure Security Enthusiast
