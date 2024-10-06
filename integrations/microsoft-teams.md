---
title: Microsoft Teams (and Office 365, Outlook, OneDrive)
sidebarTitle: Microsoft Teams
---

API configuration: [`microsoft-teams`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | ✅ |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [How to register an Application](https://go.microsoft.com/fwlink/?linkid=2083908)
-   [OAuth-related docs](https://learn.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)
-   [List of OAuth scopes](https://learn.microsoft.com/en-us/entra/identity-platform/scopes-oidc)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

This endpoint supports all Microsoft APIs available via the [Graph API](https://learn.microsoft.com/en-us/graph/overview) endpoints, which includes:

> - Microsoft 365 core services: Bookings, Calendar, Delve, Excel, Microsoft 365 compliance eDiscovery, Microsoft Search, OneDrive, OneNote, Outlook/Exchange, People (Outlook contacts), Planner, SharePoint, Teams, To Do, Viva Insights
> - Enterprise Mobility + Security services: Advanced Threat Analytics, Advanced Threat Protection, Azure Active Directory, Identity Manager, and Intune
> - Windows services: activities, devices, notifications, Universal Print
> - Dynamics 365 Business Central services


## API gotchas

* Make sure you request the `offline_access` scope to get a refresh token and keep access with your integration.


<Note>
    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/microsoft-teams.mdx)
</Note>
