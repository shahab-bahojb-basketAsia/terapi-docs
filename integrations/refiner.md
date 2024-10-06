---
title: Refiner
sidebarTitle: Refiner
---

API configuration: [`refiner`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Refiner API docs](https://refiner.io/docs/api/)
-   [Authentication and API key](https://refiner.io/docs/api/#authentication)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Refiner uses API_KEY auth mode with Authorization: Bearer `api_key` in the request header to access different endpoints.
- You can obtain your personal API key in your Refiner dashboard under `Integrations > Rest API`

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/refiner.mdx)</Note>