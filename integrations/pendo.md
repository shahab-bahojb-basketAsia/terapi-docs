---
title: Pendo
sidebarTitle: Pendo
---

API configurations: [`pendo`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Pendo Auth docs](https://engageapi.pendo.io/#getting-started)
-   [API docs](https://engageapi.pendo.io/#pendo-api-overview)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Pendo uses `API_KEY` auth mode where `x-pendo-integration-key`: `API key` is passed to the request header for Authentication.
- The main URL used to access the Pendo API corresponds to the region and web address you use when logging into Pendo's UI. The baseUrl is set to `https://app.pendo.io` but you can override it using `baseUrlOverride`.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/pendo.mdx)</Note>