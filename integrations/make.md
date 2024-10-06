---
title: Make
sidebarTitle: Make
---

API configuration: [`make`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) |  🚫 (time to contribute: &lt;48h)  |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) |  🚫 (time to contribute: &lt;48h)  |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | 🚫 (time to contribute: &lt;48h) |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

- [How to generate an authentication token](https://www.make.com/en/api-documentation/authentication-token)
- [Make Authentication](https://www.make.com/en/api-documentation/authentication)
- [Make API-rate limiting](https://www.make.com/en/api-documentation/rate-limiting)
- [API docs](https://www.make.com/en/api-documentation)
<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- When adding a new connection, you will also need to add your `environmentUrl`, this can be the link to your private instance of Make, for example, `development.make.cloud`, or the link to Make (with or without the zone, depending on a specific endpoint), for example, `eu1.make.com`. For more details, check [API structure](https://www.make.com/en/api-documentation/api-structure).

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/make.mdx)</Note>
