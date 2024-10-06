---
title: OneDrive
sidebarTitle: OneDrive
---

API configuration: [`one-drive`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://learn.microsoft.com/en-us/onedrive/developer/rest-api/getting-started/graph-oauth?view=odsp-graph-online#register-your-app)
-   [OAuth-related docs](https://learn.microsoft.com/en-us/onedrive/developer/rest-api/getting-started/authentication?view=odsp-graph-online)
-   [List of OAuth scopes](https://learn.microsoft.com/en-us/onedrive/developer/rest-api/getting-started/graph-oauth?view=odsp-graph-online#authentication-scopes)
-   [Web API docs (their REST API)](https://learn.microsoft.com/en-us/onedrive/developer/rest-api/?view=odsp-graph-online)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   To get refresh token, you will need to add **`offline_access`** to the list of your scopes.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/one-drive.mdx)</Note>
