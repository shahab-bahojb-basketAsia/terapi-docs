API configurations: [`twitter`](https://terapi.dev/providers.yaml) for OAuth1, [`twitter-v2`](https://terapi.dev/providers.yaml) for OAuth2, [`twitter-oauth2-cc`](https://terapi.dev/providers.yaml) for client_credentials flow

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

-   [OAuth2-related docs](https://developer.twitter.com/en/docs/authentication/oauth-2-0/user-access-token)
-   [OAuth2 scopes (scroll down)](https://developer.twitter.com/en/docs/authentication/oauth-2-0/authorization-code#:~:text=a%20public%20client.-,Scopes,-Scopes%20allow%20you)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   The OAuth1 and OAuth2 APIs give access to different data. Both are supported by Terapi.
-   For the OAuth 2 API: To get your `client_id` and `client_secret` you need to generate a "user authentication" within your app in the Twitter development portal.
-   Twitter also offers a client credentials token that authorizes as app instead of a user. This is listed under `twitter-oauth2-cc`. For more details check [twitter client credentials flow](https://developer.x.com/en/docs/authentication/oauth-2-0/application-only)

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/twitter.mdx)