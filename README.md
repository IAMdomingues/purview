# purview
Email Retention Policy Configuration in Microsoft Purview
Overview

This document describes the procedure for creating and configuring an email retention policy in Microsoft Purview for Exchange Online mailboxes.

Purpose

The purpose of this policy is to ensure that email data is retained according to the organization's compliance and regulatory requirements.

Prerequisites
Microsoft Purview access
Compliance Administrator or Global Administrator role
Appropriate Microsoft 365 licensing
Exchange Online mailboxes available
Scope

This retention policy applies to:
Exchange Online mailboxes
All users (or specify a particular group of users)

| Setting                | Value                  |
| ---------------------- | ---------------------- |
| Policy Name            | Email Retention Policy |
| Workload               | Exchange Email         |
| Retention Period       | 7 Years                |
| Action After Retention | Automatically Delete   |
| Scope                  | All Mailboxes          |
