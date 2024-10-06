API configurations: [`wrike`](https://terapi.dev/providers.yaml)

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

-   [Register an Application](https://www.wrike.com/frontend/apps/index.html#/api)
-   [OAuth related docs](https://developers.wrike.com/oauth-20-authorization)
-   [Wrike REST API docs](https://developers.wrike.com/overview)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   Wrike enforces a rate limit of 400 requests per minute. For more information, checkout [wrike API rate limits](https://developers.wrike.com/faq/#:~:text=Our%20current%20rate,Center%20Request).
-   You can find scopes required for each API method in their corresponding method section.
-   Currently, Terapi supports the latest version, V4, which allows access to data from only one account at a time. For more information, checkout [wrike migration from V3](https://developers.wrike.com/migration-from-api-v3/)

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/wrike.mdx)