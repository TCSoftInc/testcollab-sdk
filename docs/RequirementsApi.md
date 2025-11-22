# RequirementsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getRequirementIds**](RequirementsApi.md#getrequirementids) | **POST** /requirements/fetchIds | Get matching test cases\&#39; id |
| [**getTraceabilityMatrix**](RequirementsApi.md#gettraceabilitymatrix) | **POST** /requirements/traceability_matrix | Get Traceability Matrix |



## getRequirementIds

> FetchIdResult getRequirementIds(fetchIdPayload)

Get matching test cases\&#39; id

Get id(s) of test case(s) that match the filter criteria

### Example

```ts
import {
  Configuration,
  RequirementsApi,
} from 'testcollab-sdk';
import type { GetRequirementIdsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementsApi(config);

  const body = {
    // FetchIdPayload (optional)
    fetchIdPayload: ...,
  } satisfies GetRequirementIdsRequest;

  try {
    const data = await api.getRequirementIds(body);
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


## getTraceabilityMatrix

> TraceabilityMatrixResult getTraceabilityMatrix(traceabilityMatrixPayload)

Get Traceability Matrix

Get TraceabilityMatrix

### Example

```ts
import {
  Configuration,
  RequirementsApi,
} from 'testcollab-sdk';
import type { GetTraceabilityMatrixRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementsApi(config);

  const body = {
    // TraceabilityMatrixPayload (optional)
    traceabilityMatrixPayload: ...,
  } satisfies GetTraceabilityMatrixRequest;

  try {
    const data = await api.getTraceabilityMatrix(body);
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
| **traceabilityMatrixPayload** | [TraceabilityMatrixPayload](TraceabilityMatrixPayload.md) |  | [Optional] |

### Return type

[**TraceabilityMatrixResult**](TraceabilityMatrixResult.md)

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

