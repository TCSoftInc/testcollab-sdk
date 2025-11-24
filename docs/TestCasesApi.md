# TestCasesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTags**](TestCasesApi.md#addtags) | **POST** /tags | Add tags |
| [**bulkCopyTestCase**](TestCasesApi.md#bulkcopytestcase) | **PUT** /testcases/bulkCopy | Copy test cases |
| [**bulkDeleteTestCase**](TestCasesApi.md#bulkdeletetestcase) | **PUT** /testcases/bulkDelete | Deletes test cases |
| [**copyTestCase**](TestCasesApi.md#copytestcase) | **POST** /testcases/copy | Duplicate test case |
| [**copyToOtherProject**](TestCasesApi.md#copytootherproject) | **POST** /testcases/copyToOtherProject | Copy test cases to other project |
| [**createTestCase**](TestCasesApi.md#createtestcase) | **POST** /testcases | Create a new test case |
| [**deleteTestCase**](TestCasesApi.md#deletetestcase) | **DELETE** /testcases/{id} | Delete test case |
| [**getTestCase**](TestCasesApi.md#gettestcase) | **GET** /testcases/{id} | Get test case |
| [**getTestCaseCount**](TestCasesApi.md#gettestcasecount) | **GET** /testcases/count | Get test cases\&#39; count |
| [**getTestCaseIds**](TestCasesApi.md#gettestcaseids) | **POST** /testcases/fetchIds | Get matching test cases\&#39; id |
| [**getTestCases**](TestCasesApi.md#gettestcases) | **GET** /testcases | Get test cases |
| [**getTestCasesTags**](TestCasesApi.md#gettestcasestags) | **GET** /tags | Get tags |
| [**quickUpdateTestCases**](TestCasesApi.md#quickupdatetestcases) | **PUT** /testcases/quickUpdate | Updates test cases |
| [**revertTestCase**](TestCasesApi.md#reverttestcase) | **PUT** /testcases/{id}/revert | Revert test case to particular revision |
| [**reviewTestCase**](TestCasesApi.md#reviewtestcase) | **PUT** /testcases/{id}/review | Review action on test case |
| [**setTestCasesSortOrder**](TestCasesApi.md#settestcasessortorder) | **POST** /testcases/setSortOrder | Set sort order for test cases |
| [**testCaseBulkActions**](TestCasesApi.md#testcasebulkactions) | **POST** /testcases/bulkAction | Bulk actions on test cases |
| [**updateAttachments**](TestCasesApi.md#updateattachments) | **PUT** /testcases/{id}/updateAttachments | Update test case attachments |
| [**updateReviewer**](TestCasesApi.md#updatereviewer) | **PUT** /testcases/{id}/updateReviewer | Update test case reviewer |
| [**updateTestCase**](TestCasesApi.md#updatetestcase) | **PUT** /testcases/{id} | Updates a test case |



## addTags

> Tag addTags(testCasesTagPayload)

Add tags

Add tags for test cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { AddTagsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // TestCasesTagPayload | Tag (optional)
    testCasesTagPayload: ...,
  } satisfies AddTagsRequest;

  try {
    const data = await api.addTags(body);
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
| **testCasesTagPayload** | [TestCasesTagPayload](TestCasesTagPayload.md) | Tag | [Optional] |

### Return type

[**Tag**](Tag.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkCopyTestCase

> BulkActionResult bulkCopyTestCase(bulkCopyPayload)

Copy test cases

Bulk copy of Test Cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { BulkCopyTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // BulkCopyPayload (optional)
    bulkCopyPayload: ...,
  } satisfies BulkCopyTestCaseRequest;

  try {
    const data = await api.bulkCopyTestCase(body);
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
| **bulkCopyPayload** | [BulkCopyPayload](BulkCopyPayload.md) |  | [Optional] |

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
| **200** | Test Case copied |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bulkDeleteTestCase

> BulkActionResult bulkDeleteTestCase(bulkDeletePayload)

Deletes test cases

Bulk delete of Test Cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { BulkDeleteTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // BulkDeletePayload (optional)
    bulkDeletePayload: ...,
  } satisfies BulkDeleteTestCaseRequest;

  try {
    const data = await api.bulkDeleteTestCase(body);
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
| **bulkDeletePayload** | [BulkDeletePayload](BulkDeletePayload.md) |  | [Optional] |

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
| **200** | Test Case deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## copyTestCase

> CreateActionResult copyTestCase(testCaseCopyPayload)

Duplicate test case

Duplicates a specific test case

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { CopyTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // TestCaseCopyPayload | Test case to be duplicated (optional)
    testCaseCopyPayload: ...,
  } satisfies CopyTestCaseRequest;

  try {
    const data = await api.copyTestCase(body);
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
| **testCaseCopyPayload** | [TestCaseCopyPayload](TestCaseCopyPayload.md) | Test case to be duplicated | [Optional] |

### Return type

[**CreateActionResult**](CreateActionResult.md)

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


## copyToOtherProject

> BulkActionResult copyToOtherProject(copyToOtherProjectPayload)

Copy test cases to other project

Bulk copy of Test Cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { CopyToOtherProjectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // CopyToOtherProjectPayload (optional)
    copyToOtherProjectPayload: ...,
  } satisfies CopyToOtherProjectRequest;

  try {
    const data = await api.copyToOtherProject(body);
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
| **copyToOtherProjectPayload** | [CopyToOtherProjectPayload](CopyToOtherProjectPayload.md) |  | [Optional] |

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
| **200** | Test Case copied |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createTestCase

> TestCase createTestCase(testCasePayload)

Create a new test case

Test Case to add

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { CreateTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // TestCasePayload (optional)
    testCasePayload: ...,
  } satisfies CreateTestCaseRequest;

  try {
    const data = await api.createTestCase(body);
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
| **testCasePayload** | [TestCasePayload](TestCasePayload.md) |  | [Optional] |

### Return type

[**TestCase**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Test Case |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestCase

> object deleteTestCase(id, project)

Delete test case

Deletes a specific test case

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { DeleteTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestCaseRequest;

  try {
    const data = await api.deleteTestCase(body);
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
| **200** | Test Case deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCase

> TestCase getTestCase(id, project)

Get test case

Get details of a specific test case

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { GetTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetTestCaseRequest;

  try {
    const data = await api.getTestCase(body);
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
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**TestCase**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseCount

> Count getTestCaseCount(project, filter)

Get test cases\&#39; count

Get count of test cases for specific project

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { GetTestCaseCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetTestCaseCountRequest;

  try {
    const data = await api.getTestCaseCount(body);
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
| **200** | Count of test cases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseIds

> FetchIdResult getTestCaseIds(fetchIdPayload)

Get matching test cases\&#39; id

Get id(s) of test case(s) that match the filter criteria

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { GetTestCaseIdsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // FetchIdPayload (optional)
    fetchIdPayload: ...,
  } satisfies GetTestCaseIdsRequest;

  try {
    const data = await api.getTestCaseIds(body);
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


## getTestCases

> Array&lt;TestCase&gt; getTestCases(project, limit, start, sort, filter)

Get test cases

Get test cases specific to a project

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { GetTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestCasesRequest;

  try {
    const data = await api.getTestCases(body);
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

[**Array&lt;TestCase&gt;**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test cases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCasesTags

> Array&lt;Tag&gt; getTestCasesTags(project, limit, start, sort, filter)

Get tags

Get list of tags added for a specific project

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { GetTestCasesTagsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestCasesTagsRequest;

  try {
    const data = await api.getTestCasesTags(body);
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

[**Array&lt;Tag&gt;**](Tag.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of tags |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## quickUpdateTestCases

> BulkActionResult quickUpdateTestCases(project, testCaseQuickUpdatePayload)

Updates test cases

Test Case to update

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { QuickUpdateTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Project ID
    project: 56,
    // TestCaseQuickUpdatePayload (optional)
    testCaseQuickUpdatePayload: ...,
  } satisfies QuickUpdateTestCasesRequest;

  try {
    const data = await api.quickUpdateTestCases(body);
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
| **testCaseQuickUpdatePayload** | [TestCaseQuickUpdatePayload](TestCaseQuickUpdatePayload.md) |  | [Optional] |

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
| **200** | Updated Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## revertTestCase

> TestCase revertTestCase(id, testCaseRevertPayload)

Revert test case to particular revision

Test Case to update

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { RevertTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // TestCaseRevertPayload (optional)
    testCaseRevertPayload: ...,
  } satisfies RevertTestCaseRequest;

  try {
    const data = await api.revertTestCase(body);
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
| **testCaseRevertPayload** | [TestCaseRevertPayload](TestCaseRevertPayload.md) |  | [Optional] |

### Return type

[**TestCase**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## reviewTestCase

> GenericActionResult reviewTestCase(id, testCaseReviewPayload)

Review action on test case

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { ReviewTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // TestCaseReviewPayload (optional)
    testCaseReviewPayload: ...,
  } satisfies ReviewTestCaseRequest;

  try {
    const data = await api.reviewTestCase(body);
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
| **testCaseReviewPayload** | [TestCaseReviewPayload](TestCaseReviewPayload.md) |  | [Optional] |

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
| **200** | Result of review action |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setTestCasesSortOrder

> CreateActionResult setTestCasesSortOrder(testCasesSortOrderPayload)

Set sort order for test cases

Set sort order for test cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { SetTestCasesSortOrderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // TestCasesSortOrderPayload | Test case with new positions (optional)
    testCasesSortOrderPayload: ...,
  } satisfies SetTestCasesSortOrderRequest;

  try {
    const data = await api.setTestCasesSortOrder(body);
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
| **testCasesSortOrderPayload** | [TestCasesSortOrderPayload](TestCasesSortOrderPayload.md) | Test case with new positions | [Optional] |

### Return type

[**CreateActionResult**](CreateActionResult.md)

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


## testCaseBulkActions

> BulkActionResult testCaseBulkActions(testCaseBulkActionPayload)

Bulk actions on test cases

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { TestCaseBulkActionsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // TestCaseBulkActionPayload (optional)
    testCaseBulkActionPayload: ...,
  } satisfies TestCaseBulkActionsRequest;

  try {
    const data = await api.testCaseBulkActions(body);
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
| **testCaseBulkActionPayload** | [TestCaseBulkActionPayload](TestCaseBulkActionPayload.md) |  | [Optional] |

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
| **200** | Test case bulk action result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateAttachments

> TestCase updateAttachments(id, updateAttachmentPayload)

Update test case attachments

Test Case to update

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { UpdateAttachmentsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // UpdateAttachmentPayload (optional)
    updateAttachmentPayload: ...,
  } satisfies UpdateAttachmentsRequest;

  try {
    const data = await api.updateAttachments(body);
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
| **updateAttachmentPayload** | [UpdateAttachmentPayload](UpdateAttachmentPayload.md) |  | [Optional] |

### Return type

[**TestCase**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateReviewer

> UpdateReviewerResult updateReviewer(id, updateReviewerPayload)

Update test case reviewer

Updates the reviewer of a test case that is currently under review. This service allows changing the reviewer even when a test case is already in the review process.

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { UpdateReviewerRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // UpdateReviewerPayload (optional)
    updateReviewerPayload: ...,
  } satisfies UpdateReviewerRequest;

  try {
    const data = await api.updateReviewer(body);
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
| **updateReviewerPayload** | [UpdateReviewerPayload](UpdateReviewerPayload.md) |  | [Optional] |

### Return type

[**UpdateReviewerResult**](UpdateReviewerResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reviewer updated successfully |  -  |
| **400** | Bad Request - Missing or invalid input |  -  |
| **404** | Not Found - Resource not found |  -  |
| **500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestCase

> TestCase updateTestCase(id, testCasePayload)

Updates a test case

Test Case to update

### Example

```ts
import {
  Configuration,
  TestCasesApi,
} from '@testcollab/sdk';
import type { UpdateTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCasesApi(config);

  const body = {
    // number | Test Case ID
    id: 8.14,
    // TestCasePayload (optional)
    testCasePayload: ...,
  } satisfies UpdateTestCaseRequest;

  try {
    const data = await api.updateTestCase(body);
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
| **testCasePayload** | [TestCasePayload](TestCasePayload.md) |  | [Optional] |

### Return type

[**TestCase**](TestCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

