---
title: Google Docs  
sidebarTitle: Google Docs  
---

API configuration: [`google-docs`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can add the missing features within 48 hours; feel free to reach out in the [community](#).

## Getting started

-   [Google Docs access token specs](https://cloud.google.com/iam/docs/reference/sts/rest/v1/TopLevel/token#response-body)
-   [Google Docs OAuth scopes](https://developers.google.com/docs/api/auth#docs-scopes)
-   [Google Docs API docs](https://developers.google.com/docs/api/reference/rest)

Need assistance getting started? Visit the [community](#).

## API gotchas

-   While setting up the OAuth app, use the `https://www.googleapis.com/auth/documents` scope for extended capabilities.
-   To enable `Google Docs` in the developer console for your project, please use the following link: [Enable Google Docs API](https://console.cloud.google.com/flows/enableapi?apiid=docs.googleapis.com).
-   Different API types enforce different rate limits; ensure you monitor your usage accordingly.

Add Getting Started links and Gotchas by [editing this page](#)

