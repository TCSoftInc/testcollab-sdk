# TestCaseImportApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getImportQueueStatus**](TestCaseImportApi.md#getimportqueuestatus) | **GET** /test_cases/importQueueStatus/{importTaskID} | Returns status of the import queue |
| [**getImportSummary**](TestCaseImportApi.md#getimportsummary) | **GET** /test_cases/importSummary/{importTaskID} | Returns summary of the import task |
| [**queueImport**](TestCaseImportApi.md#queueimport) | **POST** /testcases/queueImport | Adds an import queue |



## getImportQueueStatus

> QueueStatus getImportQueueStatus(importTaskID)

Returns status of the import queue

### Example

```ts
import {
  Configuration,
  TestCaseImportApi,
} from 'testcollab-sdk';
import type { GetImportQueueStatusRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseImportApi(config);

  const body = {
    // string | Import ID (returned from queueImport operation)
    importTaskID: 1,
  } satisfies GetImportQueueStatusRequest;

  try {
    const data = await api.getImportQueueStatus(body);
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
| **importTaskID** | `string` | Import ID (returned from queueImport operation) | [Defaults to `undefined`] |

### Return type

[**QueueStatus**](QueueStatus.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue status details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getImportSummary

> ImportSummary getImportSummary(importTaskID)

Returns summary of the import task

### Example

```ts
import {
  Configuration,
  TestCaseImportApi,
} from 'testcollab-sdk';
import type { GetImportSummaryRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseImportApi(config);

  const body = {
    // string | Import ID (returned from queueImport operation)
    importTaskID: 1,
  } satisfies GetImportSummaryRequest;

  try {
    const data = await api.getImportSummary(body);
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
| **importTaskID** | `string` | Import ID (returned from queueImport operation) | [Defaults to `undefined`] |

### Return type

[**ImportSummary**](ImportSummary.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import summary |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## queueImport

> ImportActionResult queueImport(importPayload)

Adds an import queue

Adds an import queue

### Example

```ts
import {
  Configuration,
  TestCaseImportApi,
} from 'testcollab-sdk';
import type { QueueImportRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestCaseImportApi(config);

  const body = {
    // ImportPayload | Import parameters (optional)
    importPayload: ...,
  } satisfies QueueImportRequest;

  try {
    const data = await api.queueImport(body);
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
| **importPayload** | [ImportPayload](ImportPayload.md) | Import parameters | [Optional] |

### Return type

[**ImportActionResult**](ImportActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

