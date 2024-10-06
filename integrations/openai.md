---
title: OpenAI
sidebarTitle: OpenAI
---

API configuration: [`openai`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Generate an API key in your OpenAI account](https://platform.openai.com/api-keys)
-   [OpenAI API docs](https://platform.openai.com/docs/api-reference/introduction)
-   [OpenAI Authentication](https://platform.openai.com/docs/api-reference/authentication)
-   [OpenAI rate limits](https://platform.openai.com/docs/guides/rate-limits)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- OpenAI uses API_KEY auth mode with `Authorization: Bearer API_KEY` in the request header to access different endpoints.
- terapi supports automatic retries based on the `x-ratelimit-reset-requests` header from OpenAI's API. This header indicates when the request limit will reset, allowing terapi to efficiently manage API calls. Unlike `x-ratelimit-reset-tokens`, which pertains to the total token usage,`x-ratelimit-reset-requests` specifically addresses the number of API requests.
- For users associated with multiple organizations or accessing their projects via a legacy user API key, optional headers can be included to specify the organization and project for the API request. Organization IDs can be found on your [Organization settings](https://platform.openai.com/account/organization) page, while project IDs can be found on your [General settings](https://platform.openai.com/settings) page.
- This can be done at the script level:
```js
const config:ProxyConfiguration = {
    endpoint: '/v1/models',
    headers: {
        'OpenAI-Organization': $organizationId,
        'OpenAI-Project': $projectId
    }
};
```

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/openai.mdx)</Note>