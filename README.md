# Microsoft Purview – Email Retention Policy

## Overview

This document describes the procedure for creating and configuring an email retention policy in Microsoft Purview for Exchange Online mailboxes.

The configuration documented in this project was implemented as part of a corporate Microsoft 365 environment in Chile, with the objective of establishing a controlled retention period for business email data.

## Purpose

The purpose of this policy is to ensure that email data is retained according to the organization's compliance, security, operational and regulatory requirements.

The retention period was defined as part of the organization's internal information governance strategy and should be reviewed according to applicable legal, regulatory and business requirements.

## Compliance Context – Chile

The implementation considers the principles established by Chilean data protection legislation.

Chile's Law No. 19.628 regulates the protection and processing of personal data. Its principles include requirements related to appropriate processing, security and protection of personal information.

Law No. 21.719, published in 2024, establishes a modern framework for the protection and processing of personal data and creates the Chilean Data Protection Agency. The law is scheduled to enter into force on December 1, 2026.

The new framework establishes, among other principles, that personal data should only be retained for the period necessary to fulfill the purposes for which it is processed, subject to legal exceptions.

Therefore, the seven-year retention period configured in this project should be understood as an organizational retention policy and not as a general legal requirement applicable to all corporate email in Chile.

Specific regulatory or legal obligations may require longer or shorter retention periods depending on the type of information and business activity.

## International Compliance Considerations

Depending on the organization's activities, customers, locations and data flows, additional international requirements or security frameworks may apply.

Examples include:

- ISO/IEC 27001 – Information Security Management Systems
- NIST Cybersecurity Framework
- GDPR, where applicable to the processing of personal data of individuals in the European Union
- Industry-specific regulatory and contractual requirements

Retention policies should therefore be reviewed together with Legal, Compliance, Security and Information Governance teams before being applied to production environments.

## Prerequisites

- Microsoft Purview access
- Compliance Administrator or Global Administrator role
- Appropriate Microsoft 365 licensing
- Exchange Online mailboxes available

## Scope

This retention policy applies to:

- Exchange Online mailboxes
- All users, or a defined group of users depending on the organization's requirements

# Purview Configuration

| Setting | Value |
|---|---|
| Policy Name | Email Retention Policy |
| Workload | Exchange Email |
| Retention Period | 7 Years |
| Action After Retention | Automatically Delete |
| Scope | All Mailboxes |

## Governance Considerations

Before enabling automatic deletion in a production environment, organizations should validate:

- Applicable legal and regulatory retention requirements
- Litigation hold and legal hold requirements
- Internal records management policies
- Business and operational requirements
- Data classification
- Regulatory or contractual obligations
- Microsoft 365 licensing requirements
- Exceptions for specific users, groups or mailboxes

Automatic deletion should only be enabled after the retention requirements and exceptions have been formally reviewed and approved.

## Available Documents

- [Email Retention Policy](docs/Email-Retention-Policy.md)
