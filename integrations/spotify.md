API configuration: [`spotify`](https://terapi.dev/providers.yaml), [`spotify-oauth2-cc`](https://terapi.dev/providers.yaml)

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

-   [OAuth-related docs](https://developer.spotify.com/documentation/web-api/tutorials/code-flow)
-   [How Register an Application](https://developer.spotify.com/documentation/web-api/concepts/apps)
-   [Scopes](https://developer.spotify.com/documentation/web-api/concepts/scopes)
-   [Web API docs (their REST API)](https://developer.spotify.com/documentation/web-api)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas
-   Spotify offers a client credentials token that authorizes as app instead of a user. This is listed under `spotify-oauth2-cc`. For more details check [spotify client credentials flow](https://developer.spotify.com/documentation/web-api/tutorials/client-credentials-flow)
Add Getting Started links and Gotchas by [editing this page](https://github.com/nangohq/terapi/tree/master/docs-v2/integrations/all/spotify.mdx)