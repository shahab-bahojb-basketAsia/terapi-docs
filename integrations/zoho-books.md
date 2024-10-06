---
title: Zoho Books
sidebarTitle: Zoho Books
---

API configuration: [`zoho-books`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://accounts.zoho.com/developerconsole)
-   [OAuth-related docs](https://www.zoho.com/books/api/v3/oauth/#overview)
-   [List of OAuth scopes](https://www.zoho.com/books/api/v3/oauth/#overview:~:text=List%20of%20scopes%20available%20in%20Zoho%20Books%20%3A)
-   [Web API docs (their REST API)](https://www.zoho.com/books/api/v3/apicollection/#overview)

<Tip>Do you need help? Please check this link [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Depending on the region of the end-user account you are accessing, you will have to provide the region as an extension in the [connection configuration](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization). No matter whether you created your OAUth app in the EU or US, if you want to obtain the credentials of a user with an EU account, you will have to call: `terapi.auth('zoho-books', '1', {params: { extension: 'eu' }})`. You can find all the available extensions [here](https://www.zoho.com/books/api/v3/introduction/#multidc).
- You can make your OAuth app cross-data-centers with [these instructions](https://www.zoho.com/books/api/v3/introduction/#multidc). This allows a single OAuth application to make requests to the Zoho API for Zoho accounts from the US, EU, etc.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/zoho-books.mdx)</Note>
