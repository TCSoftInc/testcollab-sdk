# TestPlansApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestPlan**](TestPlansApi.md#addtestplan) | **POST** /testplans | Add new test plan |
| [**archiveTestPlan**](TestPlansApi.md#archivetestplan) | **PUT** /testplan/archive/{id} | Archive given test plan |
| [**copyTestPlan**](TestPlansApi.md#copytestplan) | **PUT** /testplan/copy/{id} | Duplicate given test plan |
| [**deleteTestPlan**](TestPlansApi.md#deletetestplan) | **DELETE** /testplans/{id} | Delete test plan |
| [**editTestPlan**](TestPlansApi.md#edittestplan) | **PUT** /testplans/{id} | Edit a test plan |
| [**getMyProgress**](TestPlansApi.md#getmyprogress) | **GET** /testplans/{id}/getMyProgress | Get specific Test Plan result |
| [**getTestPlan**](TestPlansApi.md#gettestplan) | **GET** /testplans/{id} | Get Test Plan |
| [**getTestPlanIds**](TestPlansApi.md#gettestplanids) | **POST** /testplans/fetchIds | Get matching test plans\&#39; id(s) |
| [**getTestPlans**](TestPlansApi.md#gettestplans) | **GET** /testplans | Get test plans |
| [**reopenTestPlan**](TestPlansApi.md#reopentestplan) | **PUT** /testplan/reopen/{id} | Re-open given test plan |
| [**testPlanBulkActions**](TestPlansApi.md#testplanbulkactions) | **POST** /testplans/bulkAction | Bulk actions on test plans |



## addTestPlan

> TestPlanMinified addTestPlan(testPlanPayload)

Add new test plan

Adds a new test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { AddTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // TestPlanPayload | Test plan to add (optional)
    testPlanPayload: ...,
  } satisfies AddTestPlanRequest;

  try {
    const data = await api.addTestPlan(body);
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
| **testPlanPayload** | [TestPlanPayload](TestPlanPayload.md) | Test plan to add | [Optional] |

### Return type

[**TestPlanMinified**](TestPlanMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## archiveTestPlan

> TestPlan archiveTestPlan(id)

Archive given test plan

Archives specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { ArchiveTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 8.14,
  } satisfies ArchiveTestPlanRequest;

  try {
    const data = await api.archiveTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |

### Return type

[**TestPlan**](TestPlan.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test Plan archived |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## copyTestPlan

> BulkActionResult copyTestPlan(id, duplicateTestPlanPayload)

Duplicate given test plan

Duplicates specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { CopyTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 8.14,
    // DuplicateTestPlanPayload (optional)
    duplicateTestPlanPayload: ...,
  } satisfies CopyTestPlanRequest;

  try {
    const data = await api.copyTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **duplicateTestPlanPayload** | [DuplicateTestPlanPayload](DuplicateTestPlanPayload.md) |  | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test Plan copied |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestPlan

> object deleteTestPlan(id, project)

Delete test plan

Deletes a specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { DeleteTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 1,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestPlanRequest;

  try {
    const data = await api.deleteTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## editTestPlan

> TestPlanMinified editTestPlan(id, testPlanPayload)

Edit a test plan

Edits a specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { EditTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 1,
    // TestPlanPayload | Edited Test plan (optional)
    testPlanPayload: ...,
  } satisfies EditTestPlanRequest;

  try {
    const data = await api.editTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **testPlanPayload** | [TestPlanPayload](TestPlanPayload.md) | Edited Test plan | [Optional] |

### Return type

[**TestPlanMinified**](TestPlanMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMyProgress

> ResultSummary getMyProgress(id, regression)

Get specific Test Plan result

Get results of specific test plan for logged in user

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { GetMyProgressRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 1,
    // number | Test Plan regression ID (optional)
    regression: 1,
  } satisfies GetMyProgressRequest;

  try {
    const data = await api.getMyProgress(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **regression** | `number` | Test Plan regression ID | [Optional] [Defaults to `undefined`] |

### Return type

[**ResultSummary**](ResultSummary.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test Plan Result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlan

> TestPlan getTestPlan(id, showUserTimeTaken)

Get Test Plan

Get details of specific Test Plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { GetTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 1,
    // number | Optional - Instead of test plan time taken, show time taken of specified user ID (optional)
    showUserTimeTaken: 1,
  } satisfies GetTestPlanRequest;

  try {
    const data = await api.getTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **showUserTimeTaken** | `number` | Optional - Instead of test plan time taken, show time taken of specified user ID | [Optional] [Defaults to `undefined`] |

### Return type

[**TestPlan**](TestPlan.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test Plan Details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanIds

> FetchIdResult getTestPlanIds(fetchIdPayload)

Get matching test plans\&#39; id(s)

Get id(s) of test plan(s) that match the filter criteria

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { GetTestPlanIdsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // FetchIdPayload (optional)
    fetchIdPayload: ...,
  } satisfies GetTestPlanIdsRequest;

  try {
    const data = await api.getTestPlanIds(body);
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
| **fetchIdPayload** | [FetchIdPayload](FetchIdPayload.md) |  | [Optional] |

### Return type

[**FetchIdResult**](FetchIdResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action result |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlans

> Array&lt;TestPlan&gt; getTestPlans(project, limit, start, sort, filter)

Get test plans

Get details of test plans under a specific project

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { GetTestPlansRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
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
  } satisfies GetTestPlansRequest;

  try {
    const data = await api.getTestPlans(body);
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
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlan&gt;**](TestPlan.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | list of test plans |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## reopenTestPlan

> TestPlan reopenTestPlan(id)

Re-open given test plan

Reopenes specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { ReopenTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // number | Test Plan ID
    id: 8.14,
  } satisfies ReopenTestPlanRequest;

  try {
    const data = await api.reopenTestPlan(body);
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
| **id** | `number` | Test Plan ID | [Defaults to `undefined`] |

### Return type

[**TestPlan**](TestPlan.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test Plan reopened |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## testPlanBulkActions

> BulkActionResult testPlanBulkActions(testPlanBulkActionPayload)

Bulk actions on test plans

### Example

```ts
import {
  Configuration,
  TestPlansApi,
} from 'testcollab-sdk';
import type { TestPlanBulkActionsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansApi(config);

  const body = {
    // TestPlanBulkActionPayload | Assignment criteria (optional)
    testPlanBulkActionPayload: ...,
  } satisfies TestPlanBulkActionsRequest;

  try {
    const data = await api.testPlanBulkActions(body);
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
| **testPlanBulkActionPayload** | [TestPlanBulkActionPayload](TestPlanBulkActionPayload.md) | Assignment criteria | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Assignment result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

