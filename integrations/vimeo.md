API configuration: [`vimeo`](https://terapi.dev/providers.yaml), [`vimeo-basic`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth + Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [How to register an Application](https://developer.vimeo.com/api/guides/start#register-your-app)
-   [OAuth related docs](https://developer.vimeo.com/api/authentication)
-   [List of OAuth scopes](https://developer.vimeo.com/api/authentication#table-1)
-   [Basic auth related docs](https://developer.vimeo.com/api/authentication#working-with-basic-authentication)
-   [Vimeo API docs](https://developer.vimeo.com/api/reference)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas
-   Currently `vimeo` doesn't support refresh tokens.
-   When using `vimeo-basic` authentication, add your app `client_id` as the username and `client_secret` as the password.
-   Vimeo enforces different rate limits based on the membership level. For more details check [Vimeo rate limits](https://developer.vimeo.com/guidelines/rate-limiting)
Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/vimeo.mdx)