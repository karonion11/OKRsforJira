---
layout: default
title: Marketplace Privacy & Security Draft Answers
---

# Marketplace Privacy & Security Draft Answers

This page is a working draft to support Atlassian Marketplace review responses for **OKR Tracker for Jira**.

## 1. What end-user data does the app process?

The app processes:

- Jira `accountId`
- Jira `displayName`
- Jira `avatarUrl`
- Jira `emailAddress`
- team membership mappings
- OKR content entered by customer users
- linked Jira issue keys and live Jira issue metadata used for rendering
- app permission settings and access-control assignments

## 2. What data is stored by the app?

The app stores customer tenant data in **Atlassian-hosted Forge SQL**. Stored data includes periods, teams, team memberships, objectives, key results, Jira issue link records, permission settings, and Jira `accountId` references used by those records.

## 3. Does the app store personal data outside Atlassian-hosted Forge storage/services?

Based on the current implementation, **no**. The app stores its tenant data in Atlassian-hosted Forge SQL and uses Jira Cloud APIs through Atlassian Forge.

## 4. Does the app send customer data to external third-party services?

Based on the current implementation, **no external third-party application servers are used for app data processing**. The app communicates with Jira Cloud APIs through Atlassian Forge runtime capabilities.

## 5. Does the app process email addresses?

Yes. The app processes `emailAddress` from Jira user responses to support user search and user resolution behavior.

## 6. How is access controlled?

The app enforces backend authorization rules using the current Jira user context (`context.accountId`) and app-stored permission settings. Access can be limited globally, by team scope, or by owner scope.

## 7. How can customer tenant data be deleted?

A customer may submit a verified deletion request to **support@florenco.tech**. After verification, App-stored tenant data is targeted for deletion within **30 days** using the applicable Atlassian Forge mechanisms and application-level deletion logic.

## 8. Does the app support data export?

No dedicated self-service export flow is currently documented in the app.

## 9. Where is support handled?

Support contact: **support@florenco.tech**

## 10. Public documents

- [Privacy Policy](./privacy-policy.md)
- [End User Terms of Use](./terms-of-use.md)
- [Data Retention and Deletion](./data-retention.md)
- [Support](./support.md)
