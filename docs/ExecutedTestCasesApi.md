# ExecutedTestCasesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**assignExecutedTestCase**](ExecutedTestCasesApi.md#assignexecutedtestcase) | **PUT** /executedtestcases/assign | Assign a executed test case |
| [**bulkAddExecutedTestCases**](ExecutedTestCasesApi.md#bulkaddexecutedtestcases) | **POST** /testplans/executedtestcaseBulkAdd | Add test case to testplan |
| [**bulkAddExecutedTestCasesOLD**](ExecutedTestCasesApi.md#bulkaddexecutedtestcasesold) | **PUT** /executedtestcases/{id}/bulkAdd | Add executed test case for testplan |
| [**createExecutedTestCase**](ExecutedTestCasesApi.md#createexecutedtestcase) | **POST** /executedtestcases | Create a new executed test case |
| [**deleteExecutedTestCase**](ExecutedTestCasesApi.md#deleteexecutedtestcase) | **DELETE** /executedtestcases/{id} | Deletes executed test case |
| [**getExecutedTestCase**](ExecutedTestCasesApi.md#getexecutedtestcase) | **GET** /executedtestcases/{id} | Get executed test case |
| [**getExecutedTestCaseCount**](ExecutedTestCasesApi.md#getexecutedtestcasecount) | **GET** /executedtestcases/count | Get count of executed test cases |
| [**getExecutedTestCases**](ExecutedTestCasesApi.md#getexecutedtestcases) | **GET** /executedtestcases | Get list of executed test cases |
| [**updateExecutedTestCase**](ExecutedTestCasesApi.md#updateexecutedtestcase) | **PUT** /executedtestcases/{id} | Updates an executed test case |
| [**updateTimeTaken**](ExecutedTestCasesApi.md#updatetimetaken) | **PUT** /executedtestcases/{id}/updateTimeTaken | Update executed test case time taken |



## assignExecutedTestCase

> ExecutedTestCase assignExecutedTestCase(executedTestCaseAssignPayload)

Assign a executed test case

Executed Test Case assign payload

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { AssignExecutedTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // ExecutedTestCaseAssignPayload (optional)
    executedTestCaseAssignPayload: ...,
  } satisfies AssignExecutedTestCaseRequest;

  try {
    const data = await api.assignExecutedTestCase(body);
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
| **executedTestCaseAssignPayload** | [ExecutedTestCaseAssignPayload](ExecutedTestCaseAssignPayload.md) |  | [Optional] |

### Return type

[**ExecutedTestCase**](ExecutedTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Executed Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkAddExecutedTestCases

> object bulkAddExecutedTestCases(executedTestCaseBulkAddPayload)

Add test case to testplan

Add (executed) test cases to testplan in bulk

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { BulkAddExecutedTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // ExecutedTestCaseBulkAddPayload (optional)
    executedTestCaseBulkAddPayload: ...,
  } satisfies BulkAddExecutedTestCasesRequest;

  try {
    const data = await api.bulkAddExecutedTestCases(body);
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
| **executedTestCaseBulkAddPayload** | [ExecutedTestCaseBulkAddPayload](ExecutedTestCaseBulkAddPayload.md) |  | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Executed result added |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkAddExecutedTestCasesOLD

> object bulkAddExecutedTestCasesOLD(id, executedTestCaseBulkAddPayload)

Add executed test case for testplan

Add executed test case for testplan

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { BulkAddExecutedTestCasesOLDRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Test Plan ID
    id: 1,
    // ExecutedTestCaseBulkAddPayload (optional)
    executedTestCaseBulkAddPayload: ...,
  } satisfies BulkAddExecutedTestCasesOLDRequest;

  try {
    const data = await api.bulkAddExecutedTestCasesOLD(body);
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
| **executedTestCaseBulkAddPayload** | [ExecutedTestCaseBulkAddPayload](ExecutedTestCaseBulkAddPayload.md) |  | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Executed result added |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createExecutedTestCase

> ExecutedTestCase createExecutedTestCase(executedTestCasePayload)

Create a new executed test case

Executed Test Case to add

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { CreateExecutedTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // ExecutedTestCasePayload (optional)
    executedTestCasePayload: ...,
  } satisfies CreateExecutedTestCaseRequest;

  try {
    const data = await api.createExecutedTestCase(body);
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
| **executedTestCasePayload** | [ExecutedTestCasePayload](ExecutedTestCasePayload.md) |  | [Optional] |

### Return type

[**ExecutedTestCase**](ExecutedTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Executed Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteExecutedTestCase

> object deleteExecutedTestCase(id)

Deletes executed test case

Deletes specific executed test case

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { DeleteExecutedTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Executed Test Case ID
    id: 8.14,
  } satisfies DeleteExecutedTestCaseRequest;

  try {
    const data = await api.deleteExecutedTestCase(body);
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
| **id** | `number` | Executed Test Case ID | [Defaults to `undefined`] |

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
| **200** | Executed Test Case deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutedTestCase

> ExecutedTestCase getExecutedTestCase(id)

Get executed test case

Get details of a specific executed test case

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { GetExecutedTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Executed Test Case ID
    id: 8.14,
  } satisfies GetExecutedTestCaseRequest;

  try {
    const data = await api.getExecutedTestCase(body);
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
| **id** | `number` | Executed Test Case ID | [Defaults to `undefined`] |

### Return type

[**ExecutedTestCase**](ExecutedTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected executed test case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutedTestCaseCount

> Count getExecutedTestCaseCount(project, filter)

Get count of executed test cases

Get count of executed test cases

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { GetExecutedTestCaseCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | filter query
    filter: filter_example,
  } satisfies GetExecutedTestCaseCountRequest;

  try {
    const data = await api.getExecutedTestCaseCount(body);
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
| **filter** | `string` | filter query | [Defaults to `undefined`] |

### Return type

[**Count**](Count.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of executed test cases |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExecutedTestCases

> Array&lt;ExecutedTestCase&gt; getExecutedTestCases(project, limit, start, sort, filter)

Get list of executed test cases

Get list of executed test cases

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { GetExecutedTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Project ID
    project: 56,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetExecutedTestCasesRequest;

  try {
    const data = await api.getExecutedTestCases(body);
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

[**Array&lt;ExecutedTestCase&gt;**](ExecutedTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of executed test cases |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateExecutedTestCase

> ExecutedTestCase updateExecutedTestCase(id, executedTestCasePayload)

Updates an executed test case

Updates an executed test case

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { UpdateExecutedTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Executed Test Case ID
    id: 8.14,
    // ExecutedTestCasePayload (optional)
    executedTestCasePayload: ...,
  } satisfies UpdateExecutedTestCaseRequest;

  try {
    const data = await api.updateExecutedTestCase(body);
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
| **id** | `number` | Executed Test Case ID | [Defaults to `undefined`] |
| **executedTestCasePayload** | [ExecutedTestCasePayload](ExecutedTestCasePayload.md) |  | [Optional] |

### Return type

[**ExecutedTestCase**](ExecutedTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Executed Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTimeTaken

> GenericActionResult updateTimeTaken(id, updateTimeTakenPayload)

Update executed test case time taken

Time taken to be increamented by

### Example

```ts
import {
  Configuration,
  ExecutedTestCasesApi,
} from '@testcollab/sdk';
import type { UpdateTimeTakenRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExecutedTestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // UpdateTimeTakenPayload (optional)
    updateTimeTakenPayload: ...,
  } satisfies UpdateTimeTakenRequest;

  try {
    const data = await api.updateTimeTaken(body);
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
| **id** | `number` | Test Case ID | [Defaults to `undefined`] |
| **updateTimeTakenPayload** | [UpdateTimeTakenPayload](UpdateTimeTakenPayload.md) |  | [Optional] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success result |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

