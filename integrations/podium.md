---
title: Podium
sidebarTitle: Podium
---

API configuration: [`podium`](https://terapi.dev/providers.yaml)

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

-   [How to Register an Application](https://docs.podium.com/docs/oauth#create-your-app)
-   [OAuth related docs](https://docs.podium.com/docs/oauth)
-   [List of OAuth Scopes](https://docs.podium.com/docs/oauth-scopes)
-   [Podium API docs](https://docs.podium.com/reference)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas
-   When creating a new connection in terapi, you will also have to provide your `apiVersion` for compatibility. For more details, please check [Podium API versioning](https://docs.podium.com/docs/api-version)
-   Podium enforces a rate limit of 300 requests per minute on most of its routes, with some exceptions.
<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/podium.mdx)</Note>