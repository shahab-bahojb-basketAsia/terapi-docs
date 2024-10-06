---
title: Salesforce
sidebarTitle: Salesforce
---

API configuration: [`salesforce`](https://terapi.dev/providers.yaml), [`salesforce-sandbox`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | ✅ |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Get a free Salesforce Developer Edition here](https://developer.salesforce.com/free-trials) (it's a free Sandbox to test your integration)
-   [Salesforce OAuth documentation](https://help.salesforce.com/s/articleView?id=sf.remoteaccess_authorization_code_credentials_flow.htm&type=5) (Step 7 contains the details of what Salesforce returns along with the token)
-   [Overview of OAuth scopes](https://help.salesforce.com/s/articleView?id=sf.connected_app_create_api_integration.htm&type=5)
-   [Web API docs (their REST API)](https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_rest_resources.html)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## Connection Configuration in terapi

Salesforce uses a different API base URL, called the `instance_url`, for each customer.

terapi automatically retrieves the `instance_url` (e.g. `https://yourInstance.salesforce.com/`) from Salesforce and stores it in the [Connection config](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization) for you.

If you use the terapi Proxy, it is automatically using the correct API base URL. But, if needed, you can retrieve the `instance_url` with the [backend SDK](/reference/sdks/node#get-a-connection-with-credentials) or [Connections API](/reference/api/connection/get).

## API gotchas

-   If you or your end-user are authorizing a Salesforce sandbox account, you must use the `salesforce-sandbox` integration in terapi.
-   Salesforce calls the `client_id` and `client_secret` as `Consumer Key` and `Consumer Secret`.
-   To enable offline data access with a refresh token, add the `refresh_token` (or its synonym, `offline_access`) scope. By default, access tokens expire in ~2h (but customers can configure this value). Also, check the "Introspect All Tokens" checkbox in your OAuth app settings on the Salesforce developer portal (Salesforce doesn't share the expiration date of access tokens. Instead, terapi needs to call the Salesforce API to check if access tokens are valid.)
-   If you encounter an error in your flow that says `invalid_client_id`, [make sure your (developer) User's password does not contain any special characters](https://developer.salesforce.com/forums/?id=906F00000009ABLIA2) (yes, really.)

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/salesforce.mdx)</Note>
