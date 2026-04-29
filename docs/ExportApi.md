# ExportApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**exportDefects**](ExportApi.md#exportdefects) | **POST** /defects/export | Export defects |
| [**exportIssues**](ExportApi.md#exportissues) | **POST** /issues/export | Export issues |
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

> ExportActionResult exportIssues(exportIssuesPayload)

Export issues

Export the list of issues (in JSON format for CSV generation)

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

[**ExportActionResult**](ExportActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Export result with header row and issue data |  -  |
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

