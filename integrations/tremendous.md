API configuration: [`tremendous`](https://terapi.dev/providers.yaml), [`tremendous-sandbox`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developers.tremendous.com/docs/oauth-20#step-1-register-a-developer-app)
-   [OAuth-related docs](https://developers.tremendous.com/docs/oauth-20)
-   [List of OAuth scopes](https://developers.tremendous.com/docs/oauth-20#scopes)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- Tremendous enforces a rate limit of 10 requests per second. For more details check [tremendous rate limits](https://developers.tremendous.com/docs/rate-limiting)
- Tremendous provides different base url for both sandbox and production environments. For more information check [tremendous sandbox environment](https://developers.tremendous.com/docs/sandbox-environment)

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/tremendous.mdx)