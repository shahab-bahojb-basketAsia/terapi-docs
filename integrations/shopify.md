---

title: Shopify
sidebarTitle: Shopify

---

API configuration: [`shopify`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [How to register an Application](https://shopify.dev/docs/apps/auth/oauth/getting-started#step-1-retrieve-client-credentials)
-   [OAuth-related docs](https://shopify.dev/docs/apps/auth/oauth)
-   [List of OAuth scopes](https://shopify.dev/docs/api/usage/access-scopes#authenticated-access-scopes)
-   [API](https://shopify.dev/docs/api/admin)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## Connection configuration in terapi

Shopify requires a user specific subdomain to run OAuth.

You should request this from the user and pass it to terapi in the `terapi.auth()` call:

```js
terapi.auth('shopify', '<CONNECTION-ID>', {params: {subdomain: '<shopify-subdomain>'}});
```

For more details, see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

_None yet, add yours!_

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/shopify.mdx)</Note>
