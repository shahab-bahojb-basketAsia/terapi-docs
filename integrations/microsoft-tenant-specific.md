---
title: Microsoft Tenant Specific Endpoints
sidebarTitle: Microsoft Tenant Specific
---

API configuration: [`microsoft-tenant-specific`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Create an Azure app registration for the specific application](https://go.microsoft.com/fwlink/?linkid=2083908).
    -   Add permissions for the appropriate app on the `API Permissions` tab
-   [OAuth-related docs](https://learn.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).
    -   See particularly the `tenant` parameter under [Request an authorization code](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-auth-code-flow#request-an-authorization-code).
        This `tenant` parameter must be provided as [extra configuration to the frontend SDK](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).
-   [List of OAuth scopes](https://learn.microsoft.com/en-us/azure/active-directory/develop/permissions-consent-overview)
    -   The specific scopes required will depend on the application being accessed.  This might use the [.default scope with the resource's identifier URI](https://learn.microsoft.com/en-us/entra/identity-platform/scopes-oidc#the-default-scope).

<Tip>Do you need help? Please check this link [community](https://terapi.dev/slack).</Tip>

This endpoint supports services authorized using an Azure App Registration in any accessible tenant, including:

> - Microsoft Dynamics 365 Finance and Operations

<Tip>You _can_ use this provider for general Microsoft Graph access (and the major Microsoft SaaS services like Teams, OneDrive, other Office 365 services, etc.) by setting the `tenant` to `common` but we recommend using the [Microsoft Teams provider](/integrations/all/microsoft-teams) instead which includes sync capability.</Tip>


## API gotchas

<Note>
    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/microsoft-tenant-specific.mdx)
</Note>
