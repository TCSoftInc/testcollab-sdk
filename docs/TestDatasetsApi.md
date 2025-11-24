# TestDatasetsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTestDataset**](TestDatasetsApi.md#createtestdataset) | **POST** /testdatasets | Create a new test dataset |
| [**deleteTestDataset**](TestDatasetsApi.md#deletetestdataset) | **DELETE** /testdatasets/{id} | Delete test dataset |
| [**getTestCaseDatasets**](TestDatasetsApi.md#gettestcasedatasets) | **GET** /testdatasets/getLatest | Get test datasets linked to a test cae |
| [**getTestDataset**](TestDatasetsApi.md#gettestdataset) | **GET** /testdatasets/{id} | Get test dataset |
| [**getTestDatasetCount**](TestDatasetsApi.md#gettestdatasetcount) | **GET** /testdatasets/count | Get test dataset count |
| [**getTestDatasets**](TestDatasetsApi.md#gettestdatasets) | **GET** /testdatasets | Get test datasets |
| [**linkTestCase**](TestDatasetsApi.md#linktestcase) | **POST** /testdatasets/link | Link test dataset to test case |
| [**unlinkTestCase**](TestDatasetsApi.md#unlinktestcase) | **POST** /testdatasets/unlink | Unlink test dataset from a test case |
| [**updateTestDataset**](TestDatasetsApi.md#updatetestdataset) | **PUT** /testdatasets/{id} | Updates a test dataset |



## createTestDataset

> TestDataset createTestDataset(testDatasetPayload)

Create a new test dataset

Test dataset to add

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { CreateTestDatasetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // TestDatasetPayload (optional)
    testDatasetPayload: ...,
  } satisfies CreateTestDatasetRequest;

  try {
    const data = await api.createTestDataset(body);
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
| **testDatasetPayload** | [TestDatasetPayload](TestDatasetPayload.md) |  | [Optional] |

### Return type

[**TestDataset**](TestDataset.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Test dataset |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestDataset

> object deleteTestDataset(id, project)

Delete test dataset

Deletes a specific test dataset

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { DeleteTestDatasetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Test dataset ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestDatasetRequest;

  try {
    const data = await api.deleteTestDataset(body);
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
| **id** | `number` | Test dataset ID | [Defaults to `undefined`] |
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
| **200** | Test dataset deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseDatasets

> Array&lt;TestDataset&gt; getTestCaseDatasets(project, testcase)

Get test datasets linked to a test cae

Get test datasets linked to a test cae

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { GetTestCaseDatasetsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number
    testcase: 8.14,
  } satisfies GetTestCaseDatasetsRequest;

  try {
    const data = await api.getTestCaseDatasets(body);
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
| **testcase** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;TestDataset&gt;**](TestDataset.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | test datasets |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestDataset

> TestDataset getTestDataset(id, project)

Get test dataset

Get details of a specific test dataset

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { GetTestDatasetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Test dataset ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetTestDatasetRequest;

  try {
    const data = await api.getTestDataset(body);
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
| **id** | `number` | Test dataset ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**TestDataset**](TestDataset.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test dataset |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestDatasetCount

> Count getTestDatasetCount(project, filter)

Get test dataset count

Get count of test datasets for specific project

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { GetTestDatasetCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetTestDatasetCountRequest;

  try {
    const data = await api.getTestDatasetCount(body);
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
| **200** | Count of test datasets |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestDatasets

> Array&lt;TestDataset&gt; getTestDatasets(project, limit, start, sort, filter)

Get test datasets

Get test datasets specific to a project

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { GetTestDatasetsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetTestDatasetsRequest;

  try {
    const data = await api.getTestDatasets(body);
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
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestDataset&gt;**](TestDataset.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test datasets |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## linkTestCase

> BulkActionResult linkTestCase(testDatasetCaseLinkPayload)

Link test dataset to test case

link a test dataset to a test case

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { LinkTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // TestDatasetCaseLinkPayload | link a test dataset to a test case (optional)
    testDatasetCaseLinkPayload: ...,
  } satisfies LinkTestCaseRequest;

  try {
    const data = await api.linkTestCase(body);
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
| **testDatasetCaseLinkPayload** | [TestDatasetCaseLinkPayload](TestDatasetCaseLinkPayload.md) | link a test dataset to a test case | [Optional] |

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


## unlinkTestCase

> BulkActionResult unlinkTestCase(testDatasetCaseLinkPayload)

Unlink test dataset from a test case

Unlink a test dataset from a test case

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { UnlinkTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // TestDatasetCaseLinkPayload | Unlink a test dataset from a test case (optional)
    testDatasetCaseLinkPayload: ...,
  } satisfies UnlinkTestCaseRequest;

  try {
    const data = await api.unlinkTestCase(body);
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
| **testDatasetCaseLinkPayload** | [TestDatasetCaseLinkPayload](TestDatasetCaseLinkPayload.md) | Unlink a test dataset from a test case | [Optional] |

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


## updateTestDataset

> TestDataset updateTestDataset(id, testDatasetPayload)

Updates a test dataset

Test dataset to update

### Example

```ts
import {
  Configuration,
  TestDatasetsApi,
} from '@testcollab/sdk';
import type { UpdateTestDatasetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestDatasetsApi(config);

  const body = {
    // number | Test dataset ID
    id: 8.14,
    // TestDatasetPayload (optional)
    testDatasetPayload: ...,
  } satisfies UpdateTestDatasetRequest;

  try {
    const data = await api.updateTestDataset(body);
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
| **id** | `number` | Test dataset ID | [Defaults to `undefined`] |
| **testDatasetPayload** | [TestDatasetPayload](TestDatasetPayload.md) |  | [Optional] |

### Return type

[**TestDataset**](TestDataset.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test dataset |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

