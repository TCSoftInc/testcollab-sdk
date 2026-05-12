# ExportApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**exportDefects**](ExportApi.md#exportdefects) | **POST** /defects/export | Export defects |
| [**exportIssues**](ExportApi.md#exportissues) | **POST** /issues/export | Enqueue an issue export |
| [**exportRequirements**](ExportApi.md#exportrequirements) | **POST** /requirements/export | Enqueue a requirement export |
| [**exportTestCases**](ExportApi.md#exporttestcases) | **POST** /testcases/export | Export test cases |



## exportDefects

> ExportActionResult exportDefects(exportDefectsPayload)

Export defects

Export the list of defects (in JSON format for CSV generation)

### Example

```ts
import {
  Configuration,
  ExportApi,
} from '@testcollab/sdk';
import type { ExportDefectsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExportApi(config);

  const body = {
    // ExportDefectsPayload (optional)
    exportDefectsPayload: ...,
  } satisfies ExportDefectsRequest;

  try {
    const data = await api.exportDefects(body);
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
| **exportDefectsPayload** | [ExportDefectsPayload](ExportDefectsPayload.md) |  | [Optional] |

### Return type

[**ExportActionResult**](ExportActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Export result with header row and defect data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## exportIssues

> ExportEnqueueResult exportIssues(exportIssuesPayload)

Enqueue an issue export

Enqueues an asynchronous issue CSV export. The response returns a queueId that the client should poll via GET /queues/{id}. When the queue row reaches status 2, queue.results contains a &#x60;url&#x60; field pointing to the generated CSV file (the file is uploaded via the configured upload provider — S3 in production, local in development).

### Example

```ts
import {
  Configuration,
  ExportApi,
} from '@testcollab/sdk';
import type { ExportIssuesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExportApi(config);

  const body = {
    // ExportIssuesPayload (optional)
    exportIssuesPayload: ...,
  } satisfies ExportIssuesRequest;

  try {
    const data = await api.exportIssues(body);
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
| **exportIssuesPayload** | [ExportIssuesPayload](ExportIssuesPayload.md) |  | [Optional] |

### Return type

[**ExportEnqueueResult**](ExportEnqueueResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Export job enqueued — poll /queues/{id} for the result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## exportRequirements

> ExportEnqueueResult exportRequirements(exportRequirementsPayload)

Enqueue a requirement export

Enqueues an asynchronous requirement CSV export. The response returns a queueId that the client should poll via GET /queues/{id}. When the queue row reaches status 2, queue.results contains a &#x60;url&#x60; field pointing to the generated CSV file.

### Example

```ts
import {
  Configuration,
  ExportApi,
} from '@testcollab/sdk';
import type { ExportRequirementsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExportApi(config);

  const body = {
    // ExportRequirementsPayload (optional)
    exportRequirementsPayload: ...,
  } satisfies ExportRequirementsRequest;

  try {
    const data = await api.exportRequirements(body);
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
| **exportRequirementsPayload** | [ExportRequirementsPayload](ExportRequirementsPayload.md) |  | [Optional] |

### Return type

[**ExportEnqueueResult**](ExportEnqueueResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Export job enqueued — poll /queues/{id} for the result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## exportTestCases

> ExportActionResult exportTestCases(exportTestCasesPayload)

Export test cases

Custom export the list of test cases (in JSON format)

### Example

```ts
import {
  Configuration,
  ExportApi,
} from '@testcollab/sdk';
import type { ExportTestCasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExportApi(config);

  const body = {
    // ExportTestCasesPayload (optional)
    exportTestCasesPayload: ...,
  } satisfies ExportTestCasesRequest;

  try {
    const data = await api.exportTestCases(body);
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
| **exportTestCasesPayload** | [ExportTestCasesPayload](ExportTestCasesPayload.md) |  | [Optional] |

### Return type

[**ExportActionResult**](ExportActionResult.md)

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

