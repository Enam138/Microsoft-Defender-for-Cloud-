# Security Recommendations Assessment

## Overview

One of the primary capabilities of Microsoft Defender for Cloud is the ability to continuously assess Azure resources and generate actionable security recommendations.

These recommendations are based on Microsoft's Cloud Security Benchmark and are designed to help organizations reduce security risks, strengthen cloud governance, and improve their overall security posture.

During this project, I reviewed each recommendation presented by Microsoft Defender for Cloud and evaluated it based on:

- Security impact
- Business relevance
- Azure architecture
- Licensing requirements
- Operational considerations

Rather than implementing every recommendation automatically, I assessed each one individually and made informed decisions based on the environment.

# Objectives

The objectives of this assessment were to:

- Review Microsoft Defender for Cloud recommendations.
- Understand the risks associated with each finding.
- Implement recommendations that improved the security posture.
- Document recommendations requiring premium services or architectural changes.
- Validate implemented security controls.

# Security Recommendations Dashboard

<img width="1600" height="760" alt="defender for cloud overview" src="https://github.com/user-attachments/assets/69341b72-f6bb-4069-8238-5efbf5a79537" />


The Recommendations dashboard categorized findings by severity and provided detailed remediation guidance for each recommendation.

This centralized view allowed me to prioritize security improvements based on their potential impact.


# Recommendation 1: Configure Security Email Notifications

## Security Risk

Without security notifications, administrators may not become aware of high-severity security alerts in a timely manner.

Delayed awareness can increase response times during security incidents.

## Implementation

I configured Microsoft Defender for Cloud email notifications to:

- Receive notifications for high-severity security alerts.
- Notify Azure subscription owners.
- Ensure security contacts were properly configured.


## Validation

After configuration, I verified that:

- Email notifications were enabled.
- Subscription owners were included.
- Security contacts were correctly configured.


**Screenshot**

<img width="1600" height="756" alt="email notify" src="https://github.com/user-attachments/assets/a23ee355-6f14-4ae6-9d6e-08eda2a5e03c" />


# Recommendation 2: Enable Diagnostic Logging for Azure Key Vault

## Security Risk

Without diagnostic logging, activities performed within Azure Key Vault cannot be centrally monitored or audited.

This limits visibility into administrative operations and security events.


## Implementation

To address this recommendation, I:

- Created a Log Analytics Workspace.
- Configured Azure Key Vault Diagnostic Settings.
- Enabled:

  - All Logs
  - All Metrics

- Forwarded logs to the Log Analytics Workspace.


## Validation

After configuration, I confirmed:

- Diagnostic settings were successfully created.
- Logs were configured to flow to Log Analytics.
- Microsoft Defender for Cloud recognized the configuration during subsequent assessments.

Because Defender assessments are performed periodically, I understood that recommendations may remain visible until the next evaluation cycle.


### Log Analytics Workspace

<img width="941" height="905" alt="log ana work" src="https://github.com/user-attachments/assets/6ee71a6d-d3cf-4cbe-8e90-5a97f77b77aa" />


### Key Vault Diagnostic Settings

<img width="942" height="910" alt="key vault diag" src="https://github.com/user-attachments/assets/9d96b752-5aa6-48cf-8c86-6329df0f1912" />


# Recommendation 3: Review Azure Storage Account Authentication

## Security Risk

Microsoft Defender for Cloud recommended reviewing Shared Key authentication for the Azure Storage Account.

Although Shared Key authentication is supported, organizations should evaluate whether Microsoft Entra ID authentication is more appropriate for their workloads.


## Assessment

I reviewed the Storage Account configuration, including:

- Secure Transfer Required
- Minimum TLS Version
- Blob Anonymous Access
- Shared Key Access

Rather than disabling Shared Key authentication without understanding application dependencies, I documented the recommendation for future evaluation.

This reflects real-world security practices where changes are evaluated before implementation.


## Validation

The storage account configuration was reviewed and documented.


**Screenshot**

<img width="1600" height="758" alt="storage account settings" src="https://github.com/user-attachments/assets/00d45b70-a152-42a3-a9a1-438831904fd6" />



# Recommendation 4: Multiple Subscription Owners

## Security Risk

Microsoft recommends having multiple subscription owners to reduce the risk of administrative lockout.


## Assessment

I reviewed Azure Role-Based Access Control (RBAC) assignments for the subscription.

The review confirmed that:

- Two Owner accounts were already assigned.

Therefore, no additional remediation was required.


## Validation

Role assignments were verified through Azure IAM.


**Screenshot**

<img width="1600" height="471" alt="owner" src="https://github.com/user-attachments/assets/2461dcc7-c60a-47e5-9fbf-17a3a630ba93" />


# Recommendation 5: Review Microsoft Defender Plans

## Security Risk

Several recommendations suggested enabling additional Microsoft Defender workload protection plans.

Examples included:

- Defender for Servers
- Defender for Storage
- Defender for Key Vault
- Defender for Databases
- Defender for Resource Manager


## Assessment

I reviewed each Defender plan individually.

Rather than enabling every premium plan, I evaluated:

- Licensing requirements
- Intended workloads
- Security benefits
- Business relevance

Since these plans require additional licensing and my project focused on Cloud Security Posture Management, I documented them as future enhancements.


## Validation

The Defender Plans configuration was reviewed and documented.


**Screenshot**

<img width="1600" height="763" alt="defender plan" src="https://github.com/user-attachments/assets/f6dc1c49-e21e-4cae-86d2-92e313f2b229" />


# Recommendations Summary

| Recommendation | Action Taken | Status |
|----------------|--------------|--------|
| Configure Email Notifications | Implemented |  Completed |
| Configure Security Contacts | Implemented |  Completed |
| Enable Key Vault Diagnostic Logging | Implemented |  Completed |
| Create Log Analytics Workspace | Implemented |  Completed |
| Review Storage Account Security | Assessed and Documented |  Completed |
| Validate Subscription Owners | Verified |  Completed |
| Review Defender Plans | Assessed and Documented |  Completed |
| Azure Firewall Recommendation | Future Enhancement |  Planned |
| Defender for Storage | Future Enhancement |  Planned |
| Defender for Servers | Future Enhancement |  Planned |
| Defender for Resource Manager | Future Enhancement |  Planned |

# Key Lessons Learned

This assessment demonstrated that Microsoft Defender for Cloud is more than a vulnerability scanner.

It acts as a decision-support platform by helping security teams identify risks, prioritize remediation activities, and continuously improve cloud security.

One of the most valuable lessons I learned was that not every recommendation should be implemented immediately.

Effective cloud security requires understanding:

- Business requirements
- Security risk
- Licensing implications
- Resource dependencies
- Operational impact

By evaluating recommendations within this broader context, I developed a more practical understanding of how Cloud Security Engineers make informed security decisions in production environments.


# Skills Demonstrated

- Microsoft Defender for Cloud
- Security Recommendations
- Risk Assessment
- Azure Security Best Practices
- Security Validation
- Azure Monitoring
- Log Analytics
- Azure Key Vault
- Azure RBAC
- Cloud Security Governance

# Conclusion

Reviewing and implementing Microsoft Defender for Cloud recommendations provided practical experience in assessing cloud security risks and prioritizing remediation efforts.

Rather than simply following recommendations, I learned how to evaluate security findings, validate existing configurations, implement meaningful improvements, and document future enhancements based on business needs and licensing considerations.

This process reflects the decision-making approach used by Cloud Security Engineers to continuously strengthen Azure environments while balancing security, operational requirements, and cost.
