# ExecutionCommentsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addExecutionComment**](ExecutionCommentsApi.md#addexecutioncomment) | **POST** /executioncomments | Adds a new execution comment |
| [**deleteExecutionComment**](ExecutionCommentsApi.md#deleteexecutioncomment) | **DELETE** /executioncomments/{id} | Deletes given execution comment |
| [**getExecutionComment**](ExecutionCommentsApi.md#getexecutioncomment) | **GET** /executioncomments/{id} | Get execution comment |
| [**getExecutionComments**](ExecutionCommentsApi.md#getexecutioncomments) | **GET** /executioncomments | Get Execution comments |
| [**getExecutionCommentsCount**](ExecutionCommentsApi.md#getexecutioncommentscount) | **GET** /executioncomments/count | Get count of execution comments |
| [**updateExecutionComment**](ExecutionCommentsApi.md#updateexecutioncomment) | **PUT** /executioncomments/{id} | Updates a execution comment |



## addExecutionComment

> ExecutionComment addExecutionComment(executionCommentPayload)

Adds a new execution comment

Adds a new execution comment

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { AddExecutionCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // ExecutionCommentPayload | Comment to add (optional)
    executionCommentPayload: ...,
  } satisfies AddExecutionCommentRequest;

  try {
    const data = await api.addExecutionComment(body);
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
| **executionCommentPayload** | [ExecutionCommentPayload](ExecutionCommentPayload.md) | Comment to add | [Optional] |

### Return type

[**ExecutionComment**](ExecutionComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created ExecutionComment |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteExecutionComment

> object deleteExecutionComment(id, project)

Deletes given execution comment

Deletes a specific execution comment

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { DeleteExecutionCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // number | Execution Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteExecutionCommentRequest;

  try {
    const data = await api.deleteExecutionComment(body);
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
| **id** | `number` | Execution Comment ID | [Defaults to `undefined`] |
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
| **200** | Execution Comment deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutionComment

> ExecutionComment getExecutionComment(id, project)

Get execution comment

Get execution comment

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { GetExecutionCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // number | Execution Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetExecutionCommentRequest;

  try {
    const data = await api.getExecutionComment(body);
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
| **id** | `number` | Execution Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**ExecutionComment**](ExecutionComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected execution |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutionComments

> Array&lt;ExecutionComment&gt; getExecutionComments(executedTestCase, project, limit, start, sort, filter)

Get Execution comments

Get Execution comments

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { GetExecutionCommentsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // number | Execution ID
    executedTestCase: 1,
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetExecutionCommentsRequest;

  try {
    const data = await api.getExecutionComments(body);
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
| **executedTestCase** | `number` | Execution ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ExecutionComment&gt;**](ExecutionComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test plan comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutionCommentsCount

> Count getExecutionCommentsCount(project, executedTestCase)

Get count of execution comments

Get execution comments\&#39; count

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { GetExecutionCommentsCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Execution ID
    executedTestCase: 8.14,
  } satisfies GetExecutionCommentsCountRequest;

  try {
    const data = await api.getExecutionCommentsCount(body);
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
| **executedTestCase** | `number` | Execution ID | [Defaults to `undefined`] |

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
| **200** | Count of execution comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateExecutionComment

> ExecutionComment updateExecutionComment(id, executionCommentPayload)

Updates a execution comment

Execution to update

### Example

```ts
import {
  Configuration,
  ExecutionCommentsApi,
} from 'testcollab-sdk';
import type { UpdateExecutionCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutionCommentsApi(config);

  const body = {
    // number | Execution Comment ID
    id: 8.14,
    // ExecutionCommentPayload (optional)
    executionCommentPayload: ...,
  } satisfies UpdateExecutionCommentRequest;

  try {
    const data = await api.updateExecutionComment(body);
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
| **id** | `number` | Execution Comment ID | [Defaults to `undefined`] |
| **executionCommentPayload** | [ExecutionCommentPayload](ExecutionCommentPayload.md) |  | [Optional] |

### Return type

[**ExecutionComment**](ExecutionComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Execution comment |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

