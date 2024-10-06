API configuration: [`stripe-app`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://stripe.com/docs/stripe-apps)
-   [OAuth-related docs](https://stripe.com/docs/stripe-apps/api-authentication/oauth)
-   [List of OAuth scopes](https://stripe.com/docs/stripe-apps/reference/permissions)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## Connection configuration in Terapi for external test apps

- If you are using the "External Test" version of your app, Stripe requires you to use a temporary id to identify your application. See the [docs](https://stripe.com/docs/stripe-apps/api-authentication/oauth#install-app) for more information.

- In this case, you must use the `stripe-app-sandbox` integration in Terapi, and add the temporary ID to the `appDomain` field in the connection params.

```js
terapi.auth('stripe-app-sandbox', '', {params: {appDomain: ''}});
```

## API gotchas

- Stripe app does not return an `expire_at` or `expire_in` value during the exchange of a code for an access token. However, according to the [docs](https://docs.stripe.com/stripe-apps/api-authentication/oauth#refresh-access-token), access tokens expire in one hour, while refresh tokens expire in one year

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/stripe-app.mdx)