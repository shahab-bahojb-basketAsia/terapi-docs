API configurations: [`wordpress`](https://terapi.dev/providers.yaml)

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

-   [Register an Application](https://developer.wordpress.com/apps/)
-   [OAuth related docs](https://developer.wordpress.com/docs/oauth2/)
-   [List of OAuth scopes](https://developer.wordpress.com/docs/oauth2/#token-scope)
-   [Wordpress REST API docs](https://developer.wordpress.com/docs/api/)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas
- The `access_token` generated is long lived and thus don't expire. For more details check [required parameters](https://developer.wordpress.com/docs/oauth2/#1-required-parameters-)
Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/wordpress.mdx)