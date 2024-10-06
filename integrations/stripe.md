API configuration: [`stripe`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://dashboard.stripe.com/account/applications/settings)
-   [OAuth-related docs](https://stripe.com/docs/connect/oauth-reference)
-   [List of OAuth scopes](https://stripe.com/docs/connect/oauth-reference#:~:text=if%20not%20provided.-,scope,-Optional)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- Specific parameters for the OAuth flow can be used for testing according to the [documentation](https://stripe.com/docs/connect/testing).

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/stripe.mdx)