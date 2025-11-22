# TestCaseRevisionsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTestCaseRevision**](TestCaseRevisionsApi.md#createtestcaserevision) | **POST** /testcaserevisions | Create a new test case revision |
| [**deleteTestCaseRevision**](TestCaseRevisionsApi.md#deletetestcaserevision) | **DELETE** /testcaserevisions/{id} | Delete test case revision |
| [**getTestCaseLatestRevision**](TestCaseRevisionsApi.md#gettestcaselatestrevision) | **GET** /testcaserevisions/getLatest | Get latest test case revision |
| [**getTestCaseRevision**](TestCaseRevisionsApi.md#gettestcaserevision) | **GET** /testcaserevisions/{id} | Get test case revision |
| [**getTestCaseRevisionCount**](TestCaseRevisionsApi.md#gettestcaserevisioncount) | **GET** /testcaserevisions/count | Get test case revisions\&#39; count |
| [**getTestCaseRevisions**](TestCaseRevisionsApi.md#gettestcaserevisions) | **GET** /testcaserevisions | Get test case revisions |
| [**updateTestCaseRevision**](TestCaseRevisionsApi.md#updatetestcaserevision) | **PUT** /testcaserevisions/{id} | Updates a test case revision |



## createTestCaseRevision

> TestCaseRevision createTestCaseRevision(testCaseRevisionPayload)

Create a new test case revision

Test Case Revision to add

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { CreateTestCaseRevisionRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // TestCaseRevisionPayload (optional)
    testCaseRevisionPayload: ...,
  } satisfies CreateTestCaseRevisionRequest;

  try {
    const data = await api.createTestCaseRevision(body);
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
| **testCaseRevisionPayload** | [TestCaseRevisionPayload](TestCaseRevisionPayload.md) |  | [Optional] |

### Return type

[**TestCaseRevision**](TestCaseRevision.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Test Case Revision |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestCaseRevision

> object deleteTestCaseRevision(id)

Delete test case revision

Deletes a specific test case revision

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { DeleteTestCaseRevisionRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Test Case Revision ID
    id: 8.14,
  } satisfies DeleteTestCaseRevisionRequest;

  try {
    const data = await api.deleteTestCaseRevision(body);
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
| **id** | `number` | Test Case Revision ID | [Defaults to `undefined`] |

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
| **200** | Test Case Revision deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseLatestRevision

> TestCaseRevision getTestCaseLatestRevision(project, testcase, filter)

Get latest test case revision

Gets the latest revision for a specific test case

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { GetTestCaseLatestRevisionRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Test Case ID
    testcase: 56,
    // string | Stringified JSON object for filter (optional)
    filter: filter_example,
  } satisfies GetTestCaseLatestRevisionRequest;

  try {
    const data = await api.getTestCaseLatestRevision(body);
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
| **testcase** | `number` | Test Case ID | [Defaults to `undefined`] |
| **filter** | `string` | Stringified JSON object for filter | [Optional] [Defaults to `undefined`] |

### Return type

[**TestCaseRevision**](TestCaseRevision.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Get test case revision latest |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseRevision

> TestCaseRevision getTestCaseRevision(id)

Get test case revision

Get details of a specific test case revision

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { GetTestCaseRevisionRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Test Case Revision ID
    id: 8.14,
  } satisfies GetTestCaseRevisionRequest;

  try {
    const data = await api.getTestCaseRevision(body);
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
| **id** | `number` | Test Case Revision ID | [Defaults to `undefined`] |

### Return type

[**TestCaseRevision**](TestCaseRevision.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test case revision |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseRevisionCount

> Count getTestCaseRevisionCount(project, filter)

Get test case revisions\&#39; count

Get count of test case revisions according to the filter criteria

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { GetTestCaseRevisionCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetTestCaseRevisionCountRequest;

  try {
    const data = await api.getTestCaseRevisionCount(body);
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
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |

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
| **200** | Count of test case revisions |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseRevisions

> Array&lt;TestCaseRevision&gt; getTestCaseRevisions(testcase, project, limit, start, sort, filter)

Get test case revisions

Get list of revisions a test case has been through

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { GetTestCaseRevisionsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Test Case ID
    testcase: 56,
    // number | Project ID (optional)
    project: 56,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestCaseRevisionsRequest;

  try {
    const data = await api.getTestCaseRevisions(body);
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
| **testcase** | `number` | Test Case ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestCaseRevision&gt;**](TestCaseRevision.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test case revisions |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestCaseRevision

> TestCaseRevision updateTestCaseRevision(id, testCaseRevisionPayload)

Updates a test case revision

Test Case Revision to update

### Example

```ts
import {
  Configuration,
  TestCaseRevisionsApi,
} from 'testcollab-sdk';
import type { UpdateTestCaseRevisionRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseRevisionsApi(config);

  const body = {
    // number | Test Case Revision ID
    id: 8.14,
    // TestCaseRevisionPayload (optional)
    testCaseRevisionPayload: ...,
  } satisfies UpdateTestCaseRevisionRequest;

  try {
    const data = await api.updateTestCaseRevision(body);
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
| **id** | `number` | Test Case Revision ID | [Defaults to `undefined`] |
| **testCaseRevisionPayload** | [TestCaseRevisionPayload](TestCaseRevisionPayload.md) |  | [Optional] |

### Return type

[**TestCaseRevision**](TestCaseRevision.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Case Revision |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

