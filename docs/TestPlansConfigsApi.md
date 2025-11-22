# TestPlansConfigsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestPlanConfig**](TestPlansConfigsApi.md#addtestplanconfig) | **POST** /testplanconfigurations | Add test plan config(s) |
| [**editTestPlanConfigs**](TestPlansConfigsApi.md#edittestplanconfigs) | **PUT** /testplanconfigurations | Edit test plan config(s) |
| [**getTestPlanConfig**](TestPlansConfigsApi.md#gettestplanconfig) | **GET** /testplanconfigurations/{id} | Get test plan configuration(s) |
| [**getTestPlanConfigs**](TestPlansConfigsApi.md#gettestplanconfigs) | **GET** /testplanconfigurations | Get test plan configs |



## addTestPlanConfig

> Array&lt;TestPlanConfiguration&gt; addTestPlanConfig(testPlanConfigurationPayload)

Add test plan config(s)

Add new configuration(s) to a test plan

### Example

```ts
import {
  Configuration,
  TestPlansConfigsApi,
} from 'testcollab-sdk';
import type { AddTestPlanConfigRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansConfigsApi(config);

  const body = {
    // TestPlanConfigurationPayload | Config to add (optional)
    testPlanConfigurationPayload: ...,
  } satisfies AddTestPlanConfigRequest;

  try {
    const data = await api.addTestPlanConfig(body);
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
| **testPlanConfigurationPayload** | [TestPlanConfigurationPayload](TestPlanConfigurationPayload.md) | Config to add | [Optional] |

### Return type

[**Array&lt;TestPlanConfiguration&gt;**](TestPlanConfiguration.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## editTestPlanConfigs

> Array&lt;TestPlanConfiguration&gt; editTestPlanConfigs(testPlanConfigurationsPayload)

Edit test plan config(s)

Edit test plan configurations(s)

### Example

```ts
import {
  Configuration,
  TestPlansConfigsApi,
} from 'testcollab-sdk';
import type { EditTestPlanConfigsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansConfigsApi(config);

  const body = {
    // TestPlanConfigurationsPayload | Config(s) to edit (optional)
    testPlanConfigurationsPayload: ...,
  } satisfies EditTestPlanConfigsRequest;

  try {
    const data = await api.editTestPlanConfigs(body);
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
| **testPlanConfigurationsPayload** | [TestPlanConfigurationsPayload](TestPlanConfigurationsPayload.md) | Config(s) to edit | [Optional] |

### Return type

[**Array&lt;TestPlanConfiguration&gt;**](TestPlanConfiguration.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanConfig

> TestPlanConfiguration getTestPlanConfig(id)

Get test plan configuration(s)

Get list of configuration(s) added for a test plan

### Example

```ts
import {
  Configuration,
  TestPlansConfigsApi,
} from 'testcollab-sdk';
import type { GetTestPlanConfigRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansConfigsApi(config);

  const body = {
    // number | Test Plan configuration ID
    id: 8.14,
  } satisfies GetTestPlanConfigRequest;

  try {
    const data = await api.getTestPlanConfig(body);
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
| **id** | `number` | Test Plan configuration ID | [Defaults to `undefined`] |

### Return type

[**TestPlanConfiguration**](TestPlanConfiguration.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | configuration |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanConfigs

> Array&lt;TestPlanConfiguration&gt; getTestPlanConfigs(project, testplan, limit, start, sort, filter)

Get test plan configs

Get configurations added for a specific test plan

### Example

```ts
import {
  Configuration,
  TestPlansConfigsApi,
} from 'testcollab-sdk';
import type { GetTestPlanConfigsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansConfigsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Test Plan ID
    testplan: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestPlanConfigsRequest;

  try {
    const data = await api.getTestPlanConfigs(body);
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
| **testplan** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlanConfiguration&gt;**](TestPlanConfiguration.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | list of configurations |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

