API configuration: [`tiktok`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [TikTok API Docs](https://developers.tiktok.com/doc/overview/)
-   [Full list of OAuth scopes](https://developers.tiktok.com/doc/tiktok-api-scopes/)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   The TikTok "App Id" is _not_ the `client_id`. TikTok calls the `client_id` the `Client key` and you should pass this value to Terapi as the `client_id`.
-   Make sure you pre-register your scopes in your app's config, otherwise the flow will fail when you ask for them.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/tiktok.mdx)