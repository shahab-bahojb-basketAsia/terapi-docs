API configuration: [`snowflake`](https://terapi.dev/providers.yaml)

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

-   [How to configure an OAUTH integration](https://docs.snowflake.com/en/user-guide/oauth-partner)
-   [OAuth-related docs](https://docs.snowflake.com/en/user-guide/oauth-intro)
-   [List of OAuth scopes](https://docs.snowflake.com/en/user-guide/oauth-custom#scope)
-   [Account Url configuration](https://docs.snowflake.com/en/user-guide/organizations-connect#label-connecting-via-url)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas
- When creating a connection use the correct scope/role that is granted to the user

    Add Getting Started links and Gotchas by [editing this page](https://github.com/nangohq/terapi/tree/master/docs-v2/integrations/all/snowflake.mdx)