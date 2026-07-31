# Architecture Overview

## Solution Architecture

This project demonstrates how Microsoft Defender for Cloud integrates with Azure services to continuously assess, monitor, and improve the security posture of a cloud environment.

Rather than operating as a standalone security tool, Microsoft Defender for Cloud collects security signals from Azure resources, evaluates configurations against Microsoft's security best practices, generates actionable recommendations, and measures the overall security posture of the subscription through Secure Score and Regulatory Compliance assessments.

The architecture combines infrastructure security, monitoring, governance, and compliance into a centralized cloud security solution.


# Architecture Diagram

<img width="1672" height="941" alt="ChatGPT Image Jul 30, 2026, 02_53_10 AM" src="https://github.com/user-attachments/assets/92e4e37f-29f4-4b73-ba5c-c388a3540474" />



# Architecture Components

## Microsoft Defender for Cloud

Microsoft Defender for Cloud serves as the central security management platform for the Azure environment.

It continuously evaluates Azure resources against Microsoft's Cloud Security Benchmark and provides recommendations to improve security.

### Responsibilities

- Continuous security assessment
- Cloud Security Posture Management (CSPM)
- Secure Score calculation
- Regulatory Compliance assessment
- Security recommendations
- Security alert generation
- Resource inventory
- Security governance


## Azure Virtual Network (VNet)

The Azure Virtual Network provides secure communication between Azure resources.

It isolates workloads within a private network and forms the foundation of the network security architecture.

### Responsibilities

- Network isolation
- Secure communication
- Private resource connectivity
- Traffic segmentation


## Network Security Groups (NSGs)

Network Security Groups protect Azure resources by filtering inbound and outbound network traffic using security rules.

In this environment, NSGs were configured to control traffic between subnets and protect internal resources.

### Responsibilities

- Access control
- Traffic filtering
- Least privilege networking
- Network segmentation


## Azure Storage Account

The Storage Account stores application data and diagnostic information.

Microsoft Defender for Cloud evaluates the storage account against Microsoft's security recommendations, including secure transfer requirements, authentication methods, and data protection settings.

### Responsibilities

- Secure data storage
- Storage security assessment
- Encryption validation
- Authentication review


## Azure Key Vault

Azure Key Vault securely stores secrets, certificates, and cryptographic keys.

During this project, diagnostic logging was enabled to improve visibility into Key Vault operations and strengthen auditing capabilities.

### Responsibilities

- Secret management
- Certificate management
- Key management
- Diagnostic logging
- Audit monitoring


## Private Endpoint

Private Endpoints provide secure access to Azure services over the Azure private network instead of the public internet.

This significantly reduces exposure to external threats.

### Responsibilities

- Private connectivity
- Eliminate public exposure
- Secure service communication


## Private DNS Zone

Private DNS Zones enable Azure resources connected through Private Endpoints to resolve service names internally.

This ensures seamless communication while keeping traffic within the Azure backbone network.

### Responsibilities

- Internal DNS resolution
- Private endpoint name resolution
- Secure networking


## Azure Monitor

Azure Monitor collects telemetry and operational data from Azure resources.

It provides the monitoring foundation used by Microsoft Defender for Cloud.

### Responsibilities

- Performance monitoring
- Resource monitoring
- Log collection
- Metrics collection


## Log Analytics Workspace

The Log Analytics Workspace acts as the centralized repository for diagnostic logs collected from Azure resources.

During this project, Azure Key Vault diagnostic logs were forwarded to this workspace for centralized monitoring and future security investigations.

### Responsibilities

- Centralized log storage
- Log analysis
- Security investigations
- Audit support


## Microsoft Entra ID

Microsoft Entra ID provides identity and access management for Azure resources.

It supports authentication, authorization, and Role-Based Access Control (RBAC), helping enforce least privilege across the environment.

### Responsibilities

- User authentication
- Identity management
- Role assignments
- Access control


# Security Assessment Flow

The following sequence describes how Microsoft Defender for Cloud continuously evaluates the Azure environment.

1. Azure resources generate security telemetry and configuration data.

2. Azure Monitor collects logs, metrics, and operational events.

3. Diagnostic logs from Azure Key Vault are forwarded to the Log Analytics Workspace.

4. Microsoft Defender for Cloud continuously evaluates Azure resources against Microsoft's Cloud Security Benchmark.

5. Defender calculates the Secure Score based on implemented security controls.

6. Security recommendations are generated for identified risks and configuration improvements.

7. Regulatory Compliance assessments map Azure resources against Microsoft Cloud Security Benchmark controls.

8. Administrators review recommendations and implement appropriate remediation actions.

9. Microsoft Defender for Cloud reassesses the environment after configuration changes.

10. Secure Score and compliance results are updated to reflect the current security posture.


# Security Features Demonstrated

This architecture demonstrates several Azure security capabilities, including:

- Cloud Security Posture Management (CSPM)
- Secure Score evaluation
- Regulatory Compliance assessment
- Continuous security monitoring
- Centralized logging
- Diagnostic logging
- Identity and access management
- Network segmentation
- Secure secret management
- Risk assessment
- Governance


# Design Considerations

During implementation, I evaluated each recommendation before making configuration changes.

Rather than enabling every available feature, I focused on implementing controls that improved the security posture while remaining within the scope of the available Azure services and licensing.

Premium Microsoft Defender workload protection plans, such as Defender for Servers and Defender for Storage, were reviewed and documented as future enhancements because they require additional licensing.

This approach reflects how cloud security decisions are made in real-world environments, where security improvements must be balanced with operational requirements and cost considerations.


# Conclusion

The architecture demonstrates how Microsoft Defender for Cloud integrates with Azure services to provide continuous visibility into cloud security.

By combining security assessments, centralized monitoring, compliance evaluation, and governance, the solution helps organizations proactively identify risks, strengthen security controls, and improve their overall cloud security posture.
