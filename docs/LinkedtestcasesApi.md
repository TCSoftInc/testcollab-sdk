# LinkedtestcasesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkLinkTestCase**](LinkedtestcasesApi.md#bulklinktestcase) | **POST** /linkedtestcases/bulkLink | Link bulk test cases |
| [**createLinkedTestcase**](LinkedtestcasesApi.md#createlinkedtestcase) | **POST** /linkedtestcases | Create a new linked project |
| [**getLinkedTestCases**](LinkedtestcasesApi.md#getlinkedtestcases) | **GET** /linkedtestcases | Get list of linked test cases |



## bulkLinkTestCase

> BulkActionResult bulkLinkTestCase(bulkLinkTestCasesPayload)

Link bulk test cases

Bulk copy of Test Cases

### Example

```ts
import {
  Configuration,
  LinkedtestcasesApi,
} from '@testcollab/sdk';
import type { BulkLinkTestCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new LinkedtestcasesApi(config);

  const body = {
    // BulkLinkTestCasesPayload (optional)
    bulkLinkTestCasesPayload: ...,
  } satisfies BulkLinkTestCaseRequest;

  try {
    const data = await api.bulkLinkTestCase(body);
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
| **bulkLinkTestCasesPayload** | [BulkLinkTestCasesPayload](BulkLinkTestCasesPayload.md) |  | [Optional] |

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
| **200** | Test Cases Linked |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createLinkedTestcase

> LinkedtestcasePayload createLinkedTestcase(linkedtestcasePayload)

Create a new linked project

Linked test case to add

### Example

```ts
import {
  Configuration,
  LinkedtestcasesApi,
} from '@testcollab/sdk';
import type { CreateLinkedTestcaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new LinkedtestcasesApi(config);

  const body = {
    // LinkedtestcasePayload (optional)
    linkedtestcasePayload: ...,
  } satisfies CreateLinkedTestcaseRequest;

  try {
    const data = await api.createLinkedTestcase(body);
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
| **linkedtestcasePayload** | [LinkedtestcasePayload](LinkedtestcasePayload.md) |  | [Optional] |

### Return type

[**LinkedtestcasePayload**](LinkedtestcasePayload.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Linked test case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getLinkedTestCases

> Array&lt;Linkedtestcase&gt; getLinkedTestCases(company, limit, start, sort, filter)

Get list of linked test cases

Get list of linked test cases

### Example

```ts
import {
  Configuration,
  LinkedtestcasesApi,
} from '@testcollab/sdk';
import type { GetLinkedTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new LinkedtestcasesApi(config);

  const body = {
    // number | Company ID
    company: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetLinkedTestCasesRequest;

  try {
    const data = await api.getLinkedTestCases(body);
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
| **company** | `number` | Company ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Linkedtestcase&gt;**](Linkedtestcase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Linked test cases |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

