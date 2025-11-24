# TestplansCommentsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestPlanComment**](TestplansCommentsApi.md#addtestplancomment) | **POST** /testplancomments | Add test plan comment |
| [**deleteTestPlanComment**](TestplansCommentsApi.md#deletetestplancomment) | **DELETE** /testplancomments/{id} | Delete test plan comment |
| [**getTestPlanComment**](TestplansCommentsApi.md#gettestplancomment) | **GET** /testplancomments/{id} | Get test plan comment |
| [**getTestPlanComments**](TestplansCommentsApi.md#gettestplancomments) | **GET** /testplancomments | Get test plan comments |
| [**getTestPlanCommentsCount**](TestplansCommentsApi.md#gettestplancommentscount) | **GET** /testplancomments/count | Get test plan comments\&#39; count |
| [**updateTestPlanComment**](TestplansCommentsApi.md#updatetestplancomment) | **PUT** /testplancomments/{id} | Updates a test plan comment |



## addTestPlanComment

> TestPlanComment addTestPlanComment(testPlanCommentPayload)

Add test plan comment

Adds a new test plan comment

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { AddTestPlanCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // TestPlanCommentPayload | Comment to add (optional)
    testPlanCommentPayload: ...,
  } satisfies AddTestPlanCommentRequest;

  try {
    const data = await api.addTestPlanComment(body);
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
| **testPlanCommentPayload** | [TestPlanCommentPayload](TestPlanCommentPayload.md) | Comment to add | [Optional] |

### Return type

[**TestPlanComment**](TestPlanComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created TestPlanComment |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestPlanComment

> object deleteTestPlanComment(id, project)

Delete test plan comment

Deletes specific test plan comment

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { DeleteTestPlanCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // number | Test Plan Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestPlanCommentRequest;

  try {
    const data = await api.deleteTestPlanComment(body);
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
| **id** | `number` | Test Plan Comment ID | [Defaults to `undefined`] |
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
| **200** | Test Plan Comment deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanComment

> TestPlanComment getTestPlanComment(id, project)

Get test plan comment

Get specific test plan comment

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { GetTestPlanCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // number | Test Plan Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetTestPlanCommentRequest;

  try {
    const data = await api.getTestPlanComment(body);
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
| **id** | `number` | Test Plan Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**TestPlanComment**](TestPlanComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test plan |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanComments

> Array&lt;TestPlanComment&gt; getTestPlanComments(testPlan, project, limit, start, sort, filter)

Get test plan comments

Get comments for a specific test plan

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { GetTestPlanCommentsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // number | Test Plan ID
    testPlan: 1,
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
  } satisfies GetTestPlanCommentsRequest;

  try {
    const data = await api.getTestPlanComments(body);
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
| **testPlan** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlanComment&gt;**](TestPlanComment.md)

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


## getTestPlanCommentsCount

> Count getTestPlanCommentsCount(project, testPlan)

Get test plan comments\&#39; count

Get test plan comments\&#39; count

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { GetTestPlanCommentsCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Test Plan ID
    testPlan: 8.14,
  } satisfies GetTestPlanCommentsCountRequest;

  try {
    const data = await api.getTestPlanCommentsCount(body);
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
| **testPlan** | `number` | Test Plan ID | [Defaults to `undefined`] |

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
| **200** | Count of test plan comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestPlanComment

> TestPlanComment updateTestPlanComment(id, testPlanCommentPayload)

Updates a test plan comment

Test Plan to update

### Example

```ts
import {
  Configuration,
  TestplansCommentsApi,
} from '@testcollab/sdk';
import type { UpdateTestPlanCommentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplansCommentsApi(config);

  const body = {
    // number | Test Plan Comment ID
    id: 8.14,
    // TestPlanCommentPayload (optional)
    testPlanCommentPayload: ...,
  } satisfies UpdateTestPlanCommentRequest;

  try {
    const data = await api.updateTestPlanComment(body);
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
| **id** | `number` | Test Plan Comment ID | [Defaults to `undefined`] |
| **testPlanCommentPayload** | [TestPlanCommentPayload](TestPlanCommentPayload.md) |  | [Optional] |

### Return type

[**TestPlanComment**](TestPlanComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Plan comment |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

