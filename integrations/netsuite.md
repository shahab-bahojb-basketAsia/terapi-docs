---
title: Netsuite
sidebarTitle: Netsuite
---

API configuration: [`netsuite`, `netsuite-tba`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771482304.html#Enable-the-OAuth-2.0-Feature)
-   [OAuth-related docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158081944642.html#Step-One-GET-Request-to-the-Authorization-Endpoint)
-   [Scopes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158081944642.html#subsect_158091028094) (`restlets`, `rest_webservices` and/or `suite_analytics`)
-   [API endpoints](https://system.netsuite.com/help/helpcenter/en_US/APIs/REST_API_Browser/record/v1/2023.1/index.html)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## Connection configuration in terapi

Netsuite requires a user specific account id to run OAuth.

You should request this from the user and pass it to terapi in the `terapi.auth()` call:

```js
terapi.auth('netsuite', '<CONNECTION-ID>', {params: {accountId: '<netsuite-account-id>'}});
```

For more details see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

- There doesn't seem to be a way to create a Netsuite account without scheduling a call.
- The `netsuite` integration which uses OAuth 2.0 has a refresh token that has a fixed expiration of 7 days. After which point the refresh token becomes invalid and a new access token must be obtained by making users go through the authorization code flow again.
To avoid this we recommend using the machine to machine flow which is called the `netsuite-tba` integration in terapi

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/netsuite.mdx)</Note>

## Admin Setup for `netsuite-tba`
-   Ensure you have admin privileges and login to your Netsuite account and navigate to **Setup** > **Company** > **Enable Features**
-   Under the "**SuiteTalk**" header make sure the _SOAP WEB SERVICES_ and _REST WEB SERVICES_ checkboxes are checked
<Frame>
  <img src="/images/netsuite-soap-rest-checkboxes.png" />
</Frame>
-   Under the "**Manage Authentication**" header make sure the _TOKEN-BASED AUTHENTICATION_ checkbox is checked
<Frame>
  <img src="/images/netsuite-tba-checkbox.png" />
</Frame>
-   Click the save button
-   Navigate to **Setup** > **Integration** > **Manage Integrations** > **New**
-   Set the desired name of this integration
-   Enable _TOKEN-BASED AUTHENTICATION_ and disable _TBA: AUTHORIZATION FLOW_ and _AUTHORIZATION CODE GRANT_
<Frame>
  <img src="/images/netsuite-tba-configuration.png" />
</Frame>
-   Click the save button
-   The client credentials will now be displayed and be sure to copy the **Consumer Key**, **Client ID**, **Consumer Secret**, and **Client Secret**
-   Navigate to the homepage by clicking the home icon
-   At the button left corner click the **Manage Access Tokens** button
<Frame>
  <img src="/images/netsuite-create-token.png" />
</Frame>
-   Select the **Application Name** you created for this integration
-   Enter a "**Token Name**"
-   Save your new access token
-   The token credentials will now be displayed. Copy the "**Token ID**" & "**Token Secret**"
-   In terapi create a new integration using the `netsuite-tba` and leave the "Client Id" and "Client Secret" values empty.
-   Create a new connection and for the "**OAuth Client Id Override**" value paste in the
value you received from Netsuite called "**Client ID**" and for the "**OAuth Client Secret**" value paste in the value you received
from Netsuite called "**Client Secret**". For "**Token ID**" & "**Token Secret**" paste in the values you received from Netsuite
from the access token step. The account ID value can be found from your [Netsuite URL instance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498754928.html)
-   If done programmatically using the terapi frontend sdk:
```js
terapi.auth('netsuite-tba', connectionId, {
  params: { accountId: ACCOUNT_ID },
  credentials: {
    token_id: TOKEN_ID,
    token_secret: TOKEN_SECRET,
    oauth_client_id_override: CLIENT_ID,
    oauth_client_secret_override: CLIENT_SECRET,
  }
})
```