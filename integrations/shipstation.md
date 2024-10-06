---
title: ShipStation
sidebarTitle: ShipStation
---

API configuration: [`shipstation`](https://terapi.dev/providers.yaml)

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

-   [ShipStation Basic auth related docs](https://www.shipstation.com/docs/api/requirements/#authentication)
-   [ShipStation API docs](https://www.shipstation.com/docs/api/)
-   [API rate limiting](https://www.shipstation.com/docs/api/requirements/#api-rate-limits)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- ShipStation uses `Basic` auth mode to access different endpoints. Use your ShipStation `APIKey` as the username and `APISecret` as the password, both of which can be found in the API settings.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/shipstation.mdx)</Note>