---
title: Outlook
sidebarTitle: Outlook
---

API configuration: [`outlook`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://learn.microsoft.com/en-us/graph/auth-register-app-v2)
-   [OAuth related docs](https://learn.microsoft.com/en-us/graph/auth-v2-user?tabs=http#authentication-and-authorization-steps)
-   [REST API docs](https://learn.microsoft.com/en-us/outlook/rest/#outlook-rest-api-via-microsoft-graph)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   To get refresh token, you will need to add **`offline_access`** to the list of your scopes.
-   You can find permissions required for each API call in their corresponding API methods section.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/outlook.mdx)</Note>
