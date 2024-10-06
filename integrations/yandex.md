API configuration: [`yandex`](https://terapi.dev/providers.yaml)

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

-   [OAuth-related docs](https://yandex.com/dev/id/doc/en/codes/code-url)
-   [Web API docs (their REST API)](https://cloud.yandex.com/en/docs/overview/api)
-   [How Register an Application](https://yandex.com/dev/id/doc/en/register-client)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   The scopes will depend on the [services](https://cloud.yandex.com/en/services) that you are trying to access on behalf of the user.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/yandex.mdx)