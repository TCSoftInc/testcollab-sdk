# TestplanlogsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getTestPlanLogs**](TestplanlogsApi.md#gettestplanlogs) | **GET** /testplanlogs | Get testplanlogs |



## getTestPlanLogs

> Array&lt;TestPlanLog&gt; getTestPlanLogs(project, limit, start, sort, filter, testplan)

Get testplanlogs

Get logs for a specific test plan

### Example

```ts
import {
  Configuration,
  TestplanlogsApi,
} from 'testcollab-sdk';
import type { GetTestPlanLogsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestplanlogsApi(config);

  const body = {
    // number | Project ID (optional)
    project: 8.14,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
    // number | Test Plan ID (optional)
    testplan: 8.14,
  } satisfies GetTestPlanLogsRequest;

  try {
    const data = await api.getTestPlanLogs(body);
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
| **project** | `number` | Project ID | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |
| **testplan** | `number` | Test Plan ID | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlanLog&gt;**](TestPlanLog.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of testplanlogs |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

