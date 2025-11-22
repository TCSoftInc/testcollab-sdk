# SystemApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getSystemStatus**](SystemApi.md#getsystemstatus) | **GET** / | System status |



## getSystemStatus

> SystemStatus getSystemStatus(authToken)

System status

Get system status

### Example

```ts
import {
  Configuration,
  SystemApi,
} from 'testcollab-sdk';
import type { GetSystemStatusRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new SystemApi();

  const body = {
    // string | jwt token (optional)
    authToken: authToken_example,
  } satisfies GetSystemStatusRequest;

  try {
    const data = await api.getSystemStatus(body);
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
| **authToken** | `string` | jwt token | [Optional] [Defaults to `undefined`] |

### Return type

[**SystemStatus**](SystemStatus.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | System status |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

