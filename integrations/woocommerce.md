API configuration: [`woocommerce`](https://terapi.dev/providers.yaml)

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

-   [Generate Woocommerce API credentials](https://woocommerce.github.io/woocommerce-rest-api-docs/#rest-api-keys)
-   [Woocommerce basic auth related docs](https://woocommerce.github.io/woocommerce-rest-api-docs/#authentication-over-https)
-   [Woocommerce API docs](https://woocommerce.github.io/woocommerce-rest-api-docs)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- Woocommerce uses `Basic` auth mode to access different endpoints. Provide your `consumer key` as the Username value and `consumer secret` as the Password value.
- When creating a new connection, please add your `storeURL`.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/woocommerce.mdx)