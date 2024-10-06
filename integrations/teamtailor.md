API configuration: [`teamtailor`](https://terapi.dev/providers.yaml)

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

-   [Generate an API key in your Teamtailor account](https://app.teamtailor.com/app/settings/integrations/api_keys)
-   [Teamtailor API docs](https://docs.teamtailor.com)
-   [Authentication and API key scopes](https://docs.teamtailor.com/#authentication)
-   [API rate limits](https://docs.teamtailor.com/#rate-limit)
-   [API versioning](https://docs.teamtailor.com/#versioning)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- Teamtailor uses API_KEY auth mode with Authorization: Token token=`api_key` in the request header to access different endpoints.
- The rate limit allows for a maximum of 50 requests per 10 seconds.
- All API calls must have `X-Api-Version` as a header to resolve API versions.
- Teamtailor uses different domain extensions for different regions, i.e `na` for US West(Oregon) Hosted Customers. For EU(Ireland) based clients, add `api` as your extension but for US West(Oregon) based customers add `api.na` as your extension.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/teamtailor.mdx)