---
layout: default
title: Partner Security Policy
---

# Partner Security Policy

**Effective date:** April 30, 2026

This Partner Security Policy describes the security practices for **OKR Tracker for Jira** (the "App"), provided by **Individual Entrepreneur Ihor Oleksandrovych Vasylenko**, a sole proprietor registered in Ukraine ("Vendor", "we", "us", or "our").

For security questions or to report a potential security issue, contact: **ig.vasylenko2@gmail.com**.

## 1. Scope

This Policy applies to the operation of the App in **Atlassian Jira Cloud** using the **Atlassian Forge** platform.

It describes our security approach for:
- customer data processed by the App,
- App-side access controls and permissions,
- handling of security issues and incidents,
- vulnerability management practices, and
- the App's current hosting and data flow model.

## 2. Hosting Model and No External Servers

The App is built on **Atlassian Forge** and uses **Atlassian-hosted Forge infrastructure**, including **Forge SQL**.

At the time of this Policy:

- customer App data is stored within Atlassian-hosted Forge services,
- the App does **not** rely on vendor-operated external application servers to store or process customer App data,
- the App does **not** intentionally send customer App data to separate third-party infrastructure operated by us outside the Atlassian Forge platform.

This means the App's runtime and storage model is designed to avoid unnecessary external data transfers and to minimize the number of systems involved in processing customer data.

## 3. Data Access Model

The App processes data only as needed to provide OKR functionality inside Jira Cloud.

Examples include:
- Jira `accountId` values for ownership, assignee references, team membership, permissions, and access control,
- OKR records such as periods, objectives, key results, descriptions, and progress values,
- Jira issue link records and issue metadata needed to display linked issues and status context,
- user profile details returned by Jira APIs when needed for user search and identity resolution.

Access to App functionality is limited by:
- the Atlassian and Forge execution context,
- Jira user identity available in the invocation context,
- App-level authorization rules,
- App permission settings such as owner/admin assignments and access exceptions.

## 4. Security Controls

We apply reasonable technical and organizational controls appropriate for the App's size, architecture, and hosting model.

Current security controls include:

- **Atlassian-hosted platform model**  
  The App runs on Atlassian Forge and uses Atlassian-hosted services rather than vendor-managed application servers.

- **Authentication and trusted execution context**  
  Requests are processed in the Forge context associated with the current Jira user and Atlassian tenant.

- **Application authorization checks**  
  The App enforces backend authorization rules for access to data and mutations, including permission checks for administrative and team-scoped actions.

- **Least-function data processing**  
  The App is designed to process only the data needed for OKR management and related Jira integrations.

- **Data minimization in architecture**  
  The current implementation avoids unnecessary external data pipelines and avoids storing separate external customer datasets outside Atlassian-hosted services.

- **Input validation and controlled backend operations**  
  App inputs are validated at the backend boundary before write operations are executed.

- **Controlled change management**  
  Changes to App behavior and schema are made through source-controlled updates and deployment to the Forge platform.

- **Dependency and platform-based security**  
  The App relies on maintained Atlassian Forge platform components and project dependencies, which we review and update as part of ongoing maintenance.

No security measure is absolute, but we aim to apply controls proportionate to the App's design and risk profile.

## 5. Vulnerability Management

We take a reasonable and practical approach to identifying, assessing, and addressing vulnerabilities affecting the App.

Our vulnerability management practices include:

- reviewing security reports received from customers, Atlassian, researchers, or other third parties,
- assessing the potential impact and validity of reported issues,
- prioritizing remediation based on severity, exploitability, and customer impact,
- applying fixes through App updates and redeployment where appropriate,
- reviewing relevant dependency and platform updates as part of routine maintenance.

If a vulnerability is confirmed, we aim to remediate it within a timeframe appropriate to its severity and operational impact. Critical issues are prioritized ahead of normal feature work.

Security reports can be sent to: **ig.vasylenko2@gmail.com**

We ask that reporters provide enough detail to help us reproduce and assess the issue.

## 6. Incident Response

If we become aware of a security incident affecting the App, we aim to respond in a structured and reasonable manner.

Our incident response approach generally includes:

- identifying and validating the incident,
- containing the issue where possible,
- investigating scope, affected functionality, and likely impact,
- developing and deploying remediation,
- notifying affected customers or Atlassian where appropriate and where required,
- documenting the issue and incorporating lessons learned into future improvements.

For incidents involving Atlassian-hosted platform services, our response may depend in part on Atlassian platform visibility, controls, and notifications available to Forge partners.

## 7. Logging, Monitoring, and Troubleshooting

The App may use logging and operational diagnostics available through the Atlassian Forge platform to troubleshoot errors, investigate operational issues, and support security review.

We aim to use such information only as necessary for:
- maintaining the App,
- investigating suspected defects or misuse,
- supporting incident response and remediation.

## 8. Data Sharing and Third Parties

The App depends on:
- **Atlassian Forge**,
- **Jira Cloud APIs**, and
- Atlassian-hosted infrastructure required for App delivery.

Other than the Atlassian-hosted services required to operate the App, the current implementation does not intentionally transmit customer App data to vendor-operated external servers for separate processing.

We do not sell customer data.

## 9. Customer Responsibilities

Customers are responsible for their Jira configuration, user administration, and internal decisions about which users are granted access to Jira, the App, and related project content.

Customers should also review Atlassian's own security and compliance materials for the underlying Jira Cloud and Forge platform environment.

## 10. Policy Updates

We may update this Partner Security Policy from time to time to reflect changes in the App, our practices, or review requirements.

The updated version becomes effective when published on this page.

## 11. Contact

**Individual Entrepreneur Ihor Oleksandrovych Vasylenko**  
Ukraine  
Email: **ig.vasylenko2@gmail.com**
