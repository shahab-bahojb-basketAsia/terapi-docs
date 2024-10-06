API configuration: [`zendesk`](https://terapi.dev/providers.yaml)


Zendesk has two kinds of OAuth apps:
- Helpdesk/support apps
- CRM apps

Terapi currently only supports OAuth for the Helpdesk apps. If you need CRM, reach out or contribute it :)


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

-   [How to register an Application](https://support.zendesk.com/hc/en-us/articles/4408845965210-Using-OAuth-authentication-with-your-application#topic_s21_lfs_qk)
-   [List of OAuth scopes](https://support.zendesk.com/hc/en-us/articles/4408845965210#topic_gql_kbd_gt)
-   [Setting up a global oAuth client](https://developer.zendesk.com/documentation/marketplace/building-a-marketplace-app/set-up-a-global-oauth-client/)
-   [API](https://developer.zendesk.com/api-reference/)

Do you need help? Please check this link [community](https://terapi.dev/slack).


## Connection configuration in Terapi

Zendesk requires a user specific subdomain to run OAuth.

You should request this from the user and pass it to Terapi in the `terapi.auth()` call:

```js
terapi.auth('zendesk', '', {params: {subdomain: ''}});
```

For more details, see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

-   Make sure to create a Zendesk OAuth app (`https://.zendesk.com/admin/apps-integrations/apis/zendesk-api/settings`), _not_ a Zendesk Sales CRM OAuth app. 
-   Zendesk oAuth apps [must be made "global"](https://developer.zendesk.com/documentation/marketplace/building-a-marketplace-app/set-up-a-global-oauth-client/) to connect to multiple ``s.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/zendesk.mdx)