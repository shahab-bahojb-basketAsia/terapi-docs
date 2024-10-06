API configuration: [`tableau`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (Tableau)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [How to generate your Personal Access Token](https://help.tableau.com/current/pro/desktop/en-us/useracct.htm#create-and-revoke-personal-access-tokens)
-   [Auth related docs](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_concepts_auth.htm#make-a-sign-in-request-with-a-personal-access-token)
-   [API endpoints](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api.htm)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

- When creating a new Terapi connection, please supply your Token name as your PAT NAME, Token secret as your PAT SECRET, and the content URL, which is the value that appears after `/site/` in the browser address bar for Tableau Cloud, i.e `/site/terapi1ec257d4d0/user/`, would be `terapi1ec257d4d0`. This field is left blank if you are using Tableau Server.
- You will also need to provide the [version](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_concepts_versions.htm) and [server](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_concepts_auth.htm#the-sign-in-uri) name.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/tableau.mdx)