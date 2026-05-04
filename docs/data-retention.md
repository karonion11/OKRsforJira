---
layout: default
title: Data Retention and Deletion
---

# Data Retention and Deletion

**Effective date:** April 28, 2026

This page summarizes how **OKR Tracker for Jira** handles retention and deletion requests.

## What data is stored by the App

The App stores tenant data in **Atlassian-hosted Forge SQL**, including:

- periods,
- teams and team memberships,
- objectives,
- key results,
- Jira issue link records,
- permission settings,
- Jira `accountId` references used by those records.

## What data is not primarily stored as a separate database dataset by the App

The App retrieves some Jira profile and issue data on demand from Jira APIs, including display names, avatars, email addresses, and issue status metadata. This information is used to render the product experience and is not maintained by the App as a dedicated customer directory mirror in Forge SQL.

## Standard retention

Customer data remains in the App until:

- it is deleted by customer users,
- the customer uninstalls the App and platform data lifecycle handling applies, or
- we process a verified deletion request.

## Deletion on request

For verified tenant deletion requests, we aim to delete App-stored tenant data within **30 days**.

To request deletion, contact **support@florenco.tech** and include:

- Jira site URL or tenant identification,
- app name,
- contact details of the authorized requester,
- a clear statement that you request deletion of App-stored tenant data.

## Verification

Before deletion, we may request information reasonably necessary to verify that the requester is authorized to act for the customer tenant.

## How deletion is performed

Deletion is performed using the available Atlassian Forge application and administrative mechanisms applicable to the installation and the stored tenant data.

## Contact

**support@florenco.tech**
