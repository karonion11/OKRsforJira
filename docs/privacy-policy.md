---
layout: default
title: Privacy Policy
---

# Privacy Policy

**Effective date:** April 28, 2026

This Privacy Policy describes how **Individual Entrepreneur Ihor Oleksandrovych Vasylenko**, a sole proprietor registered in Ukraine ("Vendor", "we", "us", or "our"), processes information in connection with **OKR Tracker for Jira** (the "App").

If you have questions about this Privacy Policy or want to submit a privacy or deletion request, contact: **ig.vasylenko2@gmail.com**.

For information about how we protect the App and handle security matters, please see our **[Partner Security Policy](https://karonion11.github.io/OKRsforJira/partner-security-policy.html)**.

## 1. Scope

This Privacy Policy applies to customer and end-user data processed through the App when installed in Jira Cloud.

## 2. Data we process

The App processes the following categories of data:

### Data stored in Atlassian-hosted Forge SQL

- Jira `accountId` values used for ownership, assignee references, team membership, app permissions, and access control.
- Team membership mappings between teams and Jira users.
- OKR content created by customers, including periods, objectives, key results, descriptions, progress values, and team assignments.
- Jira issue link records created inside the App, including linked Jira issue keys and optional App-side team/assignee references.
- App permission settings, including owner/admin assignments and per-user access exceptions.

### Data retrieved from Jira on demand

- `displayName`
- `avatarUrl`
- `emailAddress`
- Jira issue metadata needed to render issue links and issue status context, such as issue key, summary, issue type, status, and assignee profile details

### Data not intentionally collected by the App as a separate dataset

- Payment card data
- Government identifiers
- Special category / sensitive personal data

## 3. Why we process this data

We process data only for the following purposes:

- To authenticate the current Jira user in the App context.
- To create, read, update, and delete OKR records requested by customer users.
- To enforce the App's permissions model, including team-scoped and owner-scoped access.
- To resolve and display Jira user identities in owner, assignee, and team member pickers.
- To resolve and display Jira issue link information inside the App and issue panel.
- To operate, secure, troubleshoot, and support the App.
- To comply with legal obligations or respond to verified support/privacy requests.

## 4. Legal basis and controller/processor role

For customer content processed through the App, the customer typically acts as the controller and we typically act as a processor or service provider on the customer's behalf.

For limited business contact and support communications, we may act as an independent controller where applicable.

## 5. Where data is hosted

App data is stored using **Atlassian Forge** infrastructure, including **Atlassian-hosted Forge SQL**.

Based on the current implementation of the App, customer App data is not sent to third-party external application servers operated by us outside Atlassian-hosted Forge services.

## 6. External sharing and subprocessors

We do not sell customer data.

The App relies on Atlassian-hosted Forge platform services and Jira Cloud APIs to operate. Other than Atlassian-hosted services required to provide the App, the current implementation does not intentionally transmit customer App data to external third-party processing services.

## 7. Email address usage

The App processes `emailAddress` from Jira user profile responses to support Jira user search and user resolution behavior inside the App.

At the time of this Policy, `emailAddress` is processed from Jira responses during runtime and may be returned to the App frontend as part of user objects. It is not intentionally stored as a standalone customer directory table in Forge SQL by the App.

## 8. Retention

Customer App data is retained until one of the following occurs:

- the customer deletes the data in the App,
- the App is uninstalled and platform retention handling removes the installation data, or
- we receive and verify a deletion request and complete deletion.

When we receive a verified customer deletion request for tenant App data, we aim to delete the relevant App-stored tenant data within **30 days**.

## 9. Deletion requests

To request deletion of tenant App data, contact **ig.vasylenko2@gmail.com** and provide enough information to identify the Jira site / tenant and the installation concerned.

After verification, we will use the available Atlassian Forge administrative and application-level mechanisms to delete App-stored tenant data within the stated retention window.

## 10. Security

The App uses Atlassian Forge authentication context and Atlassian-hosted storage/services. Access to App operations is controlled through the App's backend authorization model.

No security measure is absolute, but we take reasonable steps appropriate to the App's nature and hosting model. For more information about vulnerability management, incident response, security controls, and our no-external-servers architecture, see our **[Partner Security Policy](https://karonion11.github.io/OKRsforJira/partner-security-policy.html)**.

## 11. International transfers

Because Atlassian Cloud and Forge may involve processing in multiple regions depending on Atlassian infrastructure, customer data may be processed in locations used by Atlassian to provide Forge and Jira Cloud services.

## 12. Children's data

The App is intended for business use in Jira Cloud and is not directed to children.

## 13. Changes to this Policy

We may update this Privacy Policy from time to time. The updated version becomes effective when published on this page.

## 14. Contact

**Individual Entrepreneur Ihor Oleksandrovych Vasylenko**  
Ukraine  
Email: **ig.vasylenko2@gmail.com**
