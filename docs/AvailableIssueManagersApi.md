# AvailableIssueManagersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getAvailableIssueManager**](AvailableIssueManagersApi.md#getavailableissuemanager) | **GET** /availableissuemanagers/{id} | Get available issue manager |
| [**getAvailableIssueManagers**](AvailableIssueManagersApi.md#getavailableissuemanagers) | **GET** /availableissuemanagers | Get list of available issue managers |



## getAvailableIssueManager

> AvailableIssueManager getAvailableIssueManager(id)

Get available issue manager

Get details of specific issue manager

### Example

```ts
import {
  Configuration,
  AvailableIssueManagersApi,
} from '@testcollab/sdk';
import type { GetAvailableIssueManagerRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new AvailableIssueManagersApi(config);

  const body = {
    // number | Available Issue Manager ID
    id: 8.14,
  } satisfies GetAvailableIssueManagerRequest;

  try {
    const data = await api.getAvailableIssueManager(body);
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
| **id** | `number` | Available Issue Manager ID | [Defaults to `undefined`] |

### Return type

[**AvailableIssueManager**](AvailableIssueManager.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected available issue manager |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAvailableIssueManagers

> Array&lt;AvailableIssueManager&gt; getAvailableIssueManagers(project, limit, sort, start, filter)

Get list of available issue managers

Get list of available issue managers

### Example

```ts
import {
  Configuration,
  AvailableIssueManagersApi,
} from '@testcollab/sdk';
import type { GetAvailableIssueManagersRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new AvailableIssueManagersApi(config);

  const body = {
    // number | Project ID
    project: 56,
    // number | Maximum number of records (optional)
    limit: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetAvailableIssueManagersRequest;

  try {
    const data = await api.getAvailableIssueManagers(body);
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
| **limit** | `number` | Maximum number of records | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;AvailableIssueManager&gt;**](AvailableIssueManager.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of available issue managers |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

