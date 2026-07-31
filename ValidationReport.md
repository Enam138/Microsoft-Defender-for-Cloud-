# Validation Report

## Overview

After implementing the security improvements in Microsoft Defender for Cloud, I performed a series of validation checks to confirm that the configurations were successfully applied and functioning as intended.

The purpose of this validation was to ensure that the implemented security controls aligned with Microsoft's recommended security practices and that the Azure environment reflected the expected configuration.

This report summarizes the validation activities performed throughout the project.


# Validation Objectives

The validation process focused on confirming that:

- Microsoft Defender for Cloud was properly configured.
- Security recommendations were reviewed and addressed where applicable.
- Secure Score accurately reflected the security posture of the environment.
- Regulatory Compliance assessments were available.
- Azure Key Vault diagnostic logging was enabled.
- Log Analytics Workspace received diagnostic data.
- Email notifications were configured.
- Azure RBAC assignments were verified.
- Monitoring capabilities were functioning correctly.


# Validation Summary

| Configuration | Expected Result | Validation Status |
|---------------|----------------|------------------|
| Microsoft Defender for Cloud Enabled | Security posture assessment available |  Verified |
| Secure Score Dashboard | Secure Score displayed |  Verified |
| Security Recommendations | Recommendations generated |  Verified |
| Regulatory Compliance | Microsoft Cloud Security Benchmark available |  Verified |
| Log Analytics Workspace | Successfully created |  Verified |
| Azure Key Vault Diagnostic Logs | Enabled and configured |  Verified |
| Email Notifications | Enabled |  Verified |
| Subscription Owners | Two Owner accounts confirmed |  Verified |
| Defender Plans | Reviewed and documented |  Verified |


# Validation Activities

## 1. Microsoft Defender for Cloud

### Validation

I confirmed that Microsoft Defender for Cloud was enabled and actively assessing Azure resources.

The dashboard displayed:

- Secure Score
- Recommendations
- Regulatory Compliance
- Inventory
- Defender Plans
- Security Posture

### Evidence

<img width="1600" height="760" alt="defender for cloud overview" src="https://github.com/user-attachments/assets/d99b90ca-a39b-47d9-b749-f53b03dbdb59" />


## 2. Secure Score

### Validation

I reviewed the Secure Score dashboard to verify that Microsoft Defender for Cloud had successfully assessed the Azure subscription.

The dashboard displayed:

- Current Secure Score
- Improvement recommendations
- Security posture assessment

### Evidence

<img width="1600" height="761" alt="security posture" src="https://github.com/user-attachments/assets/55974c2a-bf6c-4c8d-b457-24bf536e5c4b" />


## 3. Security Recommendations

### Validation

I confirmed that Microsoft Defender for Cloud generated recommendations based on the deployed Azure resources.

Recommendations were successfully categorized and prioritized according to Microsoft's Cloud Security Benchmark.

### Evidence

<img width="1600" height="760" alt="recommendation" src="https://github.com/user-attachments/assets/4d633135-cdbc-4e64-a3d0-72c5f1f72ee3" />


## 4. Regulatory Compliance

### Validation

I verified that the Regulatory Compliance dashboard successfully evaluated the Azure subscription using the Microsoft Cloud Security Benchmark.

The dashboard displayed:

- Passed controls
- Failed controls
- Control families
- Compliance status

### Evidence

<img width="1600" height="765" alt="compliance" src="https://github.com/user-attachments/assets/a39d8c37-2a35-4603-870c-821b41076b2d" />


## 5. Log Analytics Workspace

### Validation

I confirmed that the Log Analytics Workspace was successfully created and available for collecting diagnostic logs.

### Validation Checks

- Workspace deployed successfully
- Workspace accessible
- Available for log ingestion

### Evidence

<img width="941" height="905" alt="log ana work" src="https://github.com/user-attachments/assets/ad72d6ed-2eaf-4741-ae4c-e46acab88cd3" />


## 6. Azure Key Vault Diagnostic Logging

### Validation

I confirmed that Azure Key Vault Diagnostic Settings were configured to send logs and metrics to the Log Analytics Workspace.

The following settings were enabled:

- All Logs
- All Metrics

### Evidence

<img width="942" height="910" alt="key vault diag" src="https://github.com/user-attachments/assets/a5c87c2e-0214-43f2-85cf-b1d43f1dc0b5" />


## 7. Email Notifications

### Validation

I verified that Microsoft Defender for Cloud email notifications were configured.

Validation confirmed:

- High-severity alerts enabled
- Subscription owners notified
- Security contact configured

### Evidence

<img width="1600" height="756" alt="email notify" src="https://github.com/user-attachments/assets/aa63e203-a7d4-4bfd-aec8-a060a26ce669" />


## 8. Subscription Owner Verification

### Validation

I reviewed Azure Role-Based Access Control (RBAC) assignments to verify administrative access.

Validation confirmed:

- Two Owner accounts assigned
- Recommendation satisfied

### Evidence

<img width="1600" height="471" alt="owner" src="https://github.com/user-attachments/assets/a85762ac-9477-456a-aefa-7129483b0ef1" />


## 9. Defender Plans

### Validation

I reviewed Microsoft Defender Plans to verify:

- Foundational CSPM enabled
- Microsoft Defender CSPM enabled
- Workload protection plans reviewed

Premium Defender plans were documented as future enhancements because they require additional licensing.

### Evidence

<img width="1600" height="763" alt="defender plan" src="https://github.com/user-attachments/assets/7ac31ff7-59b7-40d7-9735-1d4e4b427eb4" />


# Overall Validation Results

The project objectives were successfully achieved.

| Project Objective | Status |
|-------------------|--------|
| Assess Azure Security Posture |  Completed |
| Review Secure Score |  Completed |
| Investigate Recommendations |  Completed |
| Configure Email Notifications |  Completed |
| Create Log Analytics Workspace |  Completed |
| Enable Key Vault Diagnostic Logging |  Completed |
| Review Defender Plans |  Completed |
| Evaluate Regulatory Compliance |  Completed |


# Lessons from Validation

The validation process reinforced the importance of verifying security configurations after implementation.

One observation during the project was that Microsoft Defender for Cloud does not immediately update every recommendation after configuration changes. Some recommendations remained visible until the next assessment cycle, highlighting that Defender continuously reassesses Azure resources rather than updating instantly.

This experience emphasized the need to manually verify security configurations instead of relying solely on dashboard indicators.


# Conclusion

The validation activities confirmed that the implemented security controls were successfully applied and that Microsoft Defender for Cloud was effectively assessing the Azure environment.

By validating each configuration, I gained practical experience in confirming cloud security implementations, interpreting assessment results, and ensuring that security improvements aligned with Microsoft's recommended best practices.

This validation process reflects the operational responsibilities of Cloud Security Engineers, who must not only implement security controls but also verify their effectiveness through continuous assessment and monitoring.
