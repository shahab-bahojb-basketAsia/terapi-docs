API configuration: [`whoop`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developer.whoop.com/docs/developing/overview/)
-   [OAuth-related docs](https://developer.whoop.com/docs/developing/oauth)
-   [List of OAuth scopes](https://developer.whoop.com/api#section/Authentication/OAuth)
-   [Web API docs (their REST API)](https://developer.whoop.com/api)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- To be able to receive a refresh token, one needs to add the `offline` scope to the OAuth authorization flow. [Required Information To Refresh](https://developer.whoop.com/docs/developing/oauth#receiving-a-refresh-token)

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/whoop.mdx)