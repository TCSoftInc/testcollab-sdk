# TestPlanTestCasesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestPlanTestCases**](TestPlanTestCasesApi.md#addtestplantestcases) | **POST** /testplantestcases | Add test cases to a test plan |
| [**bulkAddTestPlanTestCases**](TestPlanTestCasesApi.md#bulkaddtestplantestcases) | **POST** /testplantestcases/bulkAdd | Bulk add test cases to a test plan |
| [**bulkDeleteTestplanCases**](TestPlanTestCasesApi.md#bulkdeletetestplancases) | **POST** /testplantestcases/bulkDelete | Update testplan test cases in bulk |
| [**bulkUpdateTestplanCases**](TestPlanTestCasesApi.md#bulkupdatetestplancases) | **POST** /testplantestcases/bulkAction | Update testplan test cases in bulk |
| [**deleteTestPlanTestCase**](TestPlanTestCasesApi.md#deletetestplantestcase) | **DELETE** /testplantestcases/{id} | Delete a test plan test case |
| [**getTestPlanSuiteTree**](TestPlanTestCasesApi.md#gettestplansuitetree) | **GET** /testplantestcases/suitetree | suite tree for test plan\&#39;s test cases |
| [**getTestPlanTestCase**](TestPlanTestCasesApi.md#gettestplantestcase) | **GET** /testplantestcases/{id} | Get test plan test case |
| [**getTestPlanTestCaseCount**](TestPlanTestCasesApi.md#gettestplantestcasecount) | **GET** /testplantestcases/count | Get test plan test cases\&#39; count |
| [**getTestPlanTestCaseIds**](TestPlanTestCasesApi.md#gettestplantestcaseids) | **POST** /testplantestcases/fetchIds | Get matching test plan test cases\&#39; id |
| [**getTestPlanTestCases**](TestPlanTestCasesApi.md#gettestplantestcases) | **GET** /testplantestcases | Get test plan test cases |
| [**setTestPlanCasesSortOrder**](TestPlanTestCasesApi.md#settestplancasessortorder) | **POST** /testplantestcases/setSortOrder | Set sort order for test cases on run page |
| [**updateTestPlanTestCase**](TestPlanTestCasesApi.md#updatetestplantestcase) | **PUT** /testplantestcases/{id} | Updates a test plan test case |



## addTestPlanTestCases

> object addTestPlanTestCases(testPlanTestCasePayload)

Add test cases to a test plan

Array of test cases IDs -or- array of filter queries

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { AddTestPlanTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // TestPlanTestCasePayload (optional)
    testPlanTestCasePayload: ...,
  } satisfies AddTestPlanTestCasesRequest;

  try {
    const data = await api.addTestPlanTestCases(body);
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
| **testPlanTestCasePayload** | [TestPlanTestCasePayload](TestPlanTestCasePayload.md) |  | [Optional] |

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
| **200** | Action status details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkAddTestPlanTestCases

> BulkActionResult bulkAddTestPlanTestCases(testPlanTestCaseBulkAddPayload)

Bulk add test cases to a test plan

Array of test cases IDs -or- array of filter queries

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { BulkAddTestPlanTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // TestPlanTestCaseBulkAddPayload (optional)
    testPlanTestCaseBulkAddPayload: ...,
  } satisfies BulkAddTestPlanTestCasesRequest;

  try {
    const data = await api.bulkAddTestPlanTestCases(body);
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
| **testPlanTestCaseBulkAddPayload** | [TestPlanTestCaseBulkAddPayload](TestPlanTestCaseBulkAddPayload.md) |  | [Optional] |

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
| **200** | Action status details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkDeleteTestplanCases

> BulkActionResult bulkDeleteTestplanCases(bulkDeleteTestplanCasesPayload)

Update testplan test cases in bulk

Update testplan test cases in bulk

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { BulkDeleteTestplanCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // BulkDeleteTestplanCasesPayload (optional)
    bulkDeleteTestplanCasesPayload: ...,
  } satisfies BulkDeleteTestplanCasesRequest;

  try {
    const data = await api.bulkDeleteTestplanCases(body);
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
| **bulkDeleteTestplanCasesPayload** | [BulkDeleteTestplanCasesPayload](BulkDeleteTestplanCasesPayload.md) |  | [Optional] |

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
| **200** | Bulk update result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkUpdateTestplanCases

> BulkActionResult bulkUpdateTestplanCases(bulkUpdateTestplanCasesPayload)

Update testplan test cases in bulk

Update testplan test cases in bulk

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { BulkUpdateTestplanCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // BulkUpdateTestplanCasesPayload (optional)
    bulkUpdateTestplanCasesPayload: ...,
  } satisfies BulkUpdateTestplanCasesRequest;

  try {
    const data = await api.bulkUpdateTestplanCases(body);
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
| **bulkUpdateTestplanCasesPayload** | [BulkUpdateTestplanCasesPayload](BulkUpdateTestplanCasesPayload.md) |  | [Optional] |

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
| **200** | Bulk update result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestPlanTestCase

> object deleteTestPlanTestCase(id, project)

Delete a test plan test case

Deletes a specific test case added for a test plan

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { DeleteTestPlanTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Test Plan Test Case ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestPlanTestCaseRequest;

  try {
    const data = await api.deleteTestPlanTestCase(body);
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
| **id** | `number` | Test Plan Test Case ID | [Defaults to `undefined`] |
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
| **200** | Test Plan Test Case deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanSuiteTree

> SuiteTree getTestPlanSuiteTree(testplan)

suite tree for test plan\&#39;s test cases

returns suite tree of execution

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { GetTestPlanSuiteTreeRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Test Plan ID
    testplan: 1,
  } satisfies GetTestPlanSuiteTreeRequest;

  try {
    const data = await api.getTestPlanSuiteTree(body);
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
| **testplan** | `number` | Test Plan ID | [Defaults to `undefined`] |

### Return type

[**SuiteTree**](SuiteTree.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | suite tree |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanTestCase

> TestPlanTestCase getTestPlanTestCase(id, project)

Get test plan test case

Get details of a specific test case added to a test plan

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { GetTestPlanTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Test Plan Test Case ID
    id: 8.14,
    // number | Project ID (optional)
    project: 8.14,
  } satisfies GetTestPlanTestCaseRequest;

  try {
    const data = await api.getTestPlanTestCase(body);
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
| **id** | `number` | Test Plan Test Case ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Optional] [Defaults to `undefined`] |

### Return type

[**TestPlanTestCase**](TestPlanTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test plan test case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanTestCaseCount

> Count getTestPlanTestCaseCount(project, filter)

Get test plan test cases\&#39; count

Get count of test cases added to a test plan

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { GetTestPlanTestCaseCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | filter query
    filter: filter_example,
  } satisfies GetTestPlanTestCaseCountRequest;

  try {
    const data = await api.getTestPlanTestCaseCount(body);
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
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of test plan test cases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanTestCaseIds

> FetchIdResult getTestPlanTestCaseIds(fetchIdPayload)

Get matching test plan test cases\&#39; id

Get id(s) of test case(s) under a test plan that match the filter criteria

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { GetTestPlanTestCaseIdsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // FetchIdPayload (optional)
    fetchIdPayload: ...,
  } satisfies GetTestPlanTestCaseIdsRequest;

  try {
    const data = await api.getTestPlanTestCaseIds(body);
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


## getTestPlanTestCases

> Array&lt;TestPlanTestCase&gt; getTestPlanTestCases(project, testplan, limit, start, sort, filter)

Get test plan test cases

Get list of test cases for a test plan

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { GetTestPlanTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Test Plan ID
    testplan: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestPlanTestCasesRequest;

  try {
    const data = await api.getTestPlanTestCases(body);
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
| **testplan** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlanTestCase&gt;**](TestPlanTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test plan test cases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setTestPlanCasesSortOrder

> BulkActionResult setTestPlanCasesSortOrder(testPlanCasesSortOrderPayload)

Set sort order for test cases on run page

Set sort order for test cases on run page

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { SetTestPlanCasesSortOrderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // TestPlanCasesSortOrderPayload | Test case with new positions (optional)
    testPlanCasesSortOrderPayload: ...,
  } satisfies SetTestPlanCasesSortOrderRequest;

  try {
    const data = await api.setTestPlanCasesSortOrder(body);
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
| **testPlanCasesSortOrderPayload** | [TestPlanCasesSortOrderPayload](TestPlanCasesSortOrderPayload.md) | Test case with new positions | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestPlanTestCase

> TestPlanTestCase updateTestPlanTestCase(id, testPlanTestCasePayload)

Updates a test plan test case

Test Plan Test Case to update

### Example

```ts
import {
  Configuration,
  TestPlanTestCasesApi,
} from '@testcollab/sdk';
import type { UpdateTestPlanTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanTestCasesApi(config);

  const body = {
    // number | Test Plan Test Case ID
    id: 8.14,
    // TestPlanTestCasePayload (optional)
    testPlanTestCasePayload: ...,
  } satisfies UpdateTestPlanTestCaseRequest;

  try {
    const data = await api.updateTestPlanTestCase(body);
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
| **id** | `number` | Test Plan Test Case ID | [Defaults to `undefined`] |
| **testPlanTestCasePayload** | [TestPlanTestCasePayload](TestPlanTestCasePayload.md) |  | [Optional] |

### Return type

[**TestPlanTestCase**](TestPlanTestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Plan Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

