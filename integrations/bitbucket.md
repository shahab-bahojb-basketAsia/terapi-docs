---
title: Bitbucket
sidebarTitle: Bitbucket
---

API configuration: `bitbucket`

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the community.

## Getting started

-   [How to register an Application](https://support.atlassian.com/bitbucket-cloud/docs/use-oauth-on-bitbucket-cloud/#Create-a-consumer)
-   [OAuth-related docs](https://support.atlassian.com/bitbucket-cloud/docs/use-oauth-on-bitbucket-cloud/)
-   [List of OAuth scopes](https://developer.atlassian.com/cloud/bitbucket/rest/intro/#authentication)
-   [Web API docs (their REST API)](https://developer.atlassian.com/cloud/bitbucket/rest/intro/#authentication_old)

Do you need help? Please check this link.

## API gotchas

-   Access tokens expire every 2 hours, you can use `terapi.getConnection()` to generate a new set of tokens.

Add Getting Started links and Gotchas by editing this page.

