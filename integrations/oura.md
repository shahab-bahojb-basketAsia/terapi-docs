---
title: Oura
sidebarTitle: Oura
---

API configuration: [`oura`](https://terapi.dev/providers.yaml)

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

-   [OAuth related docs](https://cloud.ouraring.com/docs/authentication#oauth2)
-   [How Register an Application](https://cloud.ouraring.com/docs/)
-   [Scopes](https://cloud.ouraring.com/docs/authentication#oauth2-scopes)
-   [Oura REST API](https://cloud.ouraring.com/v2/docs)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas
-   Oura enforces a rate limit of 5000 requests in a 5 minute period. If you expect your usage to exceed this rate limit, you can contact [Oura](mailto:api-support@ouraring.com)
<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/oura.mdx)</Note>