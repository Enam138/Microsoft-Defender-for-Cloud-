# Logging and Monitoring

## Overview

Effective cloud security depends on continuous monitoring and visibility into resource activity. Without comprehensive logging, organizations cannot effectively detect security incidents, investigate suspicious behavior, or meet auditing and compliance requirements.

During this project, I implemented centralized logging and monitoring capabilities using Azure Monitor, Log Analytics Workspace, Azure Key Vault Diagnostic Settings, and Microsoft Defender for Cloud email notifications.

These services work together to provide visibility into Azure resources and strengthen the overall security posture of the environment.

# Objectives

The objectives of this phase were to:

- Configure centralized log collection.
- Enable diagnostic logging for Azure Key Vault.
- Create a Log Analytics Workspace.
- Configure Microsoft Defender for Cloud email notifications.
- Improve visibility into Azure security events.
- Support future security investigations and auditing.


# Monitoring Architecture

<img width="1672" height="941" alt="ChatGPT Image Jul 30, 2026, 02_53_10 AM" src="https://github.com/user-attachments/assets/48efc5b5-2b69-4176-90ca-55a3b89e1ed4" />


The architecture illustrates how Azure services generate telemetry that is collected by Azure Monitor, stored in Log Analytics, and analyzed by Microsoft Defender for Cloud to provide security recommendations and compliance assessments.


# Azure Monitor

Azure Monitor is Microsoft's platform for collecting telemetry, performance metrics, logs, and diagnostic information from Azure resources.

It acts as the foundation for monitoring within Azure and enables organizations to observe the health, performance, and security of their cloud environments.

During this project, Azure Monitor provided the infrastructure required to collect and manage diagnostic information from Azure services.

### Key Capabilities

- Resource monitoring
- Performance metrics
- Activity logs
- Diagnostic logs
- Alert integration
- Log Analytics integration

# Log Analytics Workspace

One of the recommendations from Microsoft Defender for Cloud required enabling diagnostic logging for Azure Key Vault.

To support this recommendation, I created a dedicated Log Analytics Workspace.

The workspace serves as a centralized repository where logs from Azure resources are stored for analysis, monitoring, auditing, and future security investigations.


## Implementation

I created a Log Analytics Workspace and configured it as the destination for Azure Key Vault diagnostic logs.

This implementation established centralized logging for the project and laid the foundation for future integration with Azure Monitor alerts and Microsoft Sentinel.


## Validation

After deployment, I confirmed that:

- The Log Analytics Workspace was successfully created.
- Azure Key Vault could send diagnostic data to the workspace.
- Microsoft Defender for Cloud recognized the monitoring configuration.

### Screenshot

<img width="941" height="905" alt="log ana work" src="https://github.com/user-attachments/assets/71e748d6-644e-423c-bed9-c55fa29910b5" />


# Azure Key Vault Diagnostic Logging

Azure Key Vault stores sensitive information such as secrets, certificates, and cryptographic keys.

To improve auditing and monitoring, I enabled diagnostic logging for the Key Vault.

## Diagnostic Settings Configured

The following categories were enabled:

- All Logs
- All Metrics

The logs were configured to be forwarded to the Log Analytics Workspace.

## Why This Matters

Enabling diagnostic logging improves visibility into Key Vault activity by recording events such as:

- Administrative operations
- Secret access
- Configuration changes
- Authentication events
- Service activity

This information supports auditing, troubleshooting, and security investigations.

## Validation

After applying the configuration, I verified that:

- Diagnostic Settings were successfully created.
- Logs were configured to flow to Log Analytics.
- Microsoft Defender for Cloud reflected the updated configuration after reassessment.

### Screenshot

<img width="942" height="910" alt="key vault diag" src="https://github.com/user-attachments/assets/4664820b-aa52-4828-a094-348da362a2d4" />


# Microsoft Defender for Cloud Email Notifications

Timely notification of security events is essential for effective incident response.

To improve operational awareness, I configured Microsoft Defender for Cloud email notifications.


## Configuration

The following settings were enabled:

- Email notifications for high-severity security alerts.
- Notifications to Azure subscription owners.
- Security contact configuration.

This ensures that administrators receive alerts when Microsoft Defender for Cloud detects significant security events.

## Validation

I verified that:

- Email notifications were enabled.
- Subscription owners were configured as recipients.
- Notification settings were successfully saved.


### Screenshot

<img width="1600" height="756" alt="email notify" src="https://github.com/user-attachments/assets/258be806-da9e-435b-876b-589e87090f8e" />


# Centralized Monitoring Workflow

The monitoring process implemented during this project follows these steps:

1. Azure resources generate telemetry and security events.
2. Azure Monitor collects metrics and diagnostic data.
3. Azure Key Vault forwards diagnostic logs to the Log Analytics Workspace.
4. Microsoft Defender for Cloud analyzes resource configurations and monitoring data.
5. Security recommendations and Secure Score are updated based on assessment results.
6. Administrators receive email notifications for high-severity security alerts.

This workflow provides continuous visibility into the Azure environment and supports proactive security management.

# Benefits of Centralized Logging

Implementing centralized logging provides several advantages:

- Improved visibility into Azure resources.
- Support for security investigations.
- Centralized audit trails.
- Better troubleshooting capabilities.
- Foundation for threat detection.
- Improved compliance reporting.
- Preparation for future Microsoft Sentinel integration.

# Skills Demonstrated

Through this phase of the project, I gained hands-on experience with:

- Azure Monitor
- Log Analytics Workspace
- Diagnostic Settings
- Azure Key Vault Monitoring
- Microsoft Defender for Cloud
- Security Notifications
- Centralized Logging
- Cloud Monitoring
- Security Operations

# Lessons Learned

This implementation reinforced the importance of monitoring as a core component of cloud security.

Deploying secure infrastructure is only the first step. Organizations must also continuously collect, analyze, and review security data to identify threats, validate configurations, and maintain visibility across their cloud environments.

By configuring centralized logging and monitoring, I gained a better understanding of how cloud security engineers use Azure services to support ongoing security operations and incident response.

# Conclusion

Logging and monitoring are fundamental to maintaining a secure Azure environment.

By implementing Azure Monitor, Log Analytics Workspace, Azure Key Vault Diagnostic Settings, and Microsoft Defender for Cloud email notifications, I improved the visibility and auditability of the environment while establishing a foundation for continuous security monitoring.

This experience strengthened my understanding of how centralized monitoring supports cloud security operations, governance, and incident response in real-world Azure environments.
