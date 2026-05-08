# IssueCommentsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addIssueComment**](IssueCommentsApi.md#addissuecomment) | **POST** /issuecomments | Add issue comment |
| [**deleteIssueComment**](IssueCommentsApi.md#deleteissuecomment) | **DELETE** /issuecomments/{id} | Delete issue comment |
| [**getIssueComment**](IssueCommentsApi.md#getissuecomment) | **GET** /issuecomments/{id} | Get issue comment |
| [**getIssueComments**](IssueCommentsApi.md#getissuecomments) | **GET** /issuecomments | Get issue comments |
| [**getIssueCommentsCount**](IssueCommentsApi.md#getissuecommentscount) | **GET** /issuecomments/count | Get issue comments count |
| [**updateIssueComment**](IssueCommentsApi.md#updateissuecomment) | **PUT** /issuecomments/{id} | Updates an issue comment |



## addIssueComment

> IssueComment addIssueComment(issueCommentPayload)

Add issue comment

Adds a new comment on an issue

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { AddIssueCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // IssueCommentPayload | Comment to add (optional)
    issueCommentPayload: ...,
  } satisfies AddIssueCommentRequest;

  try {
    const data = await api.addIssueComment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **issueCommentPayload** | [IssueCommentPayload](IssueCommentPayload.md) | Comment to add | [Optional] |

### Return type

[**IssueComment**](IssueComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created IssueComment |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteIssueComment

> object deleteIssueComment(id, project)

Delete issue comment

Delete a specific comment on an issue (creator only, within 5-minute window)

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { DeleteIssueCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // number | Issue Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteIssueCommentRequest;

  try {
    const data = await api.deleteIssueComment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `number` | Issue Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Issue comment deleted |  -  |
| **403** | Forbidden - not the creator or delete window expired |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getIssueComment

> IssueComment getIssueComment(id, project)

Get issue comment

Get a specific comment on an issue

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { GetIssueCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // number | Issue Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetIssueCommentRequest;

  try {
    const data = await api.getIssueComment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `number` | Issue Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**IssueComment**](IssueComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected issue comment |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getIssueComments

> Array&lt;IssueComment&gt; getIssueComments(issue, project, limit, start, sort, filter)

Get issue comments

Get comments for a specific issue

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { GetIssueCommentsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // number | Issue ID
    issue: 1,
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetIssueCommentsRequest;

  try {
    const data = await api.getIssueComments(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **issue** | `number` | Issue ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;IssueComment&gt;**](IssueComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Issue comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getIssueCommentsCount

> Count getIssueCommentsCount(project, issue)

Get issue comments count

Get count of comments for a specific issue

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { GetIssueCommentsCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Issue ID
    issue: 8.14,
  } satisfies GetIssueCommentsCountRequest;

  try {
    const data = await api.getIssueCommentsCount(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **issue** | `number` | Issue ID | [Defaults to `undefined`] |

### Return type

[**Count**](Count.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of issue comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateIssueComment

> IssueComment updateIssueComment(id, issueCommentPayload)

Updates an issue comment

Update an issue comment (creator only, within 5-minute window)

### Example

```ts
import {
  Configuration,
  IssueCommentsApi,
} from '@testcollab/sdk';
import type { UpdateIssueCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssueCommentsApi(config);

  const body = {
    // number | Issue Comment ID
    id: 8.14,
    // IssueCommentPayload (optional)
    issueCommentPayload: ...,
  } satisfies UpdateIssueCommentRequest;

  try {
    const data = await api.updateIssueComment(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `number` | Issue Comment ID | [Defaults to `undefined`] |
| **issueCommentPayload** | [IssueCommentPayload](IssueCommentPayload.md) |  | [Optional] |

### Return type

[**IssueComment**](IssueComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated issue comment |  -  |
| **403** | Forbidden - not the creator or edit window expired |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

