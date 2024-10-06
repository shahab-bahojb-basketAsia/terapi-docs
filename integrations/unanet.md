API configuration: [`unanet`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [Unanet basic auth related docs](https://compass.cosential.com/documentation#authentication)
-   [Unanet API docs](https://compass.cosential.com/documentation)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- Unanet uses `Basic` auth mode to access different endpoints. Provide your `username` as the Username value and `password` as the Password value. Additionally, Unanet requires an API key and a firm access code when creating a new connection which are provided upon [signup](https://compass.cosential.com/home/start).

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/unanet.mdx)