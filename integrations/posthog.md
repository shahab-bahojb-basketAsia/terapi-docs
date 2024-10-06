---
title: Posthog
sidebarTitle: Posthog
---

API configurations: [`posthog`](https://terapi.dev/providers.yaml)

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

-   [How to obtain a personal API key](https://posthog.com/docs/api#how-to-obtain-a-personal-api-key)
-   [Posthog Auth docs](https://posthog.com/docs/api#how-to-authenticate-using-the-personal-api-key)
-   [API docs](https://posthog.com/docs/api)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Posthog uses `API_KEY` auth mode with `Authorization: Bearer api_key` as a request header to access different private endpoints.
- Posthog uses different domain extensions codes for different regions, i.e `us` for US cloud, `eu` for EU cloud, and your self-hosted domain for self-hosted instances.
- Posthog enforces different rate limits for different resources. For more details check [posthog rate limits](https://posthog.com/docs/api#rate-limiting)

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/posthog.mdx)</Note>