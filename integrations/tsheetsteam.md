API configuration: [`tsheetsteam`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://tsheetsteam.github.io/api_docs/#obtaining-an-api-access-token)
-   [OAuth related docs](https://tsheetsteam.github.io/api_docs/#authentication)
-   [TSheetsTeam API docs](https://tsheetsteam.github.io/api_docs/#introduction)


Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas
-   TSheetsTeam currently doesn't support scopes.
-   TSheetsTeam enforces a rate limit of 300 calls within any 5 minute time window. Rate limiting is primarily considered on a per-connection basis (per access token). For more details [TSheetsTeam request throttling](https://tsheetsteam.github.io/api_docs/#request-throttling)
Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/tsheetsteam.mdx)