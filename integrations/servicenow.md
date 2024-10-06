---
title: ServiceNow
sidebarTitle: ServiceNow
---

API configuration: [`servicenow`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://docs.servicenow.com/bundle/vancouver-application-development/page/build/pipelines-and-deployments/task/create-oauth-api-endpoints-for-external-clients.html)
-   [OAuth-related docs](https://docs.servicenow.com/bundle/vancouver-platform-security/page/administer/security/concept/c_OAuthApplications.html)
-   [List of OAuth scopes](https://docs.servicenow.com/bundle/tokyo-application-development/page/administer/security/task/t_SpecifyAnOAuthScope.html)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   For security purposes, access tokens will expire after 30 minutes by default, when this happens you can use `terapi.getConnection()` to generate a new set of tokens.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/servicenow.mdx)</Note>