---
title: Microsoft
sidebarTitle: Microsoft
---

API configuration: [`microsoft`](https://terapi.dev/providers.yaml)

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

-   [Overview of Microsoft Graph API](https://learn.microsoft.com/en-us/graph/overview)
-   [How to register an Application](https://learn.microsoft.com/en-us/graph/auth-register-app-v2)
-   [OAuth related docs](https://learn.microsoft.com/en-us/graph/auth-v2-user?tabs=http)
-   [Microsoft permissions](https://learn.microsoft.com/en-us/graph/permissions-overview?tabs=http)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   Microsoft has a unified OAuth system for their various APIs. This provider should work for most of them (e.g. Microsoft EntraID, OneNote, Onedrive, Outlook, Sharepoint Online, Microsoft Teams etc.).
-   Microsoft offers a tool that allows you to construct and perform Graph API queries and see their response for any apps on which you have an admin, developer, or tester role. For more information you can check [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).
-   You can find permissions required for each API call in their corresponding API methods section, i.e, to retrieve a list of notebook objects from Onenote, you can have a look at [List Notebooks permissions](https://learn.microsoft.com/en-us/graph/api/onenote-list-notebooks?view=graph-rest-1.0&tabs=http#permissions).
-   Please be aware that the Microsoft Graph API implements throttling to manage the volume of requests. For more information on handling throttling, refer to the [Microsoft Graph Throttling Guidance](https://learn.microsoft.com/en-us/graph/throttling).

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/microsoft.mdx)</Note>
