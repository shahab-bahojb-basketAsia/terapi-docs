---
title: Luma
sidebarTitle: Luma
---

API configuration: [`luma`](https://terapi.dev/providers.yaml)

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

-   [Generate a Luma API key.](https://lu.ma/personal/settings)
-   [Luma Authentication](https://docs.lu.ma/reference/getting-started-with-your-api#authentication)
-   [Luma API docs](https://docs.lu.ma/reference)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Luma uses API_KEY authentication mode with `x-luma-api-key: API_KEY` as a request header to access different endpoints.
- Luma enforces a rate limit of 300 requests in any 1-minute period across all endpoints. If you hit the rate limit, you will be locked out for one minute. For more details, check [Luma rate limits](https://docs.lu.ma/reference/rate-limits)

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/luma.mdx)</Note>