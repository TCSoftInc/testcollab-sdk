# TestPlanRegressionsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestPlanRegression**](TestPlanRegressionsApi.md#addtestplanregression) | **POST** /testplanregressions | Add a test plan regression |
| [**deleteTestPlanRegression**](TestPlanRegressionsApi.md#deletetestplanregression) | **DELETE** /testplanregressions/{id} | Deletes test plan regression |
| [**getTestPlanRegression**](TestPlanRegressionsApi.md#gettestplanregression) | **GET** /testplanregressions/{id} | Get test plan regression |
| [**getTestPlanRegressionCount**](TestPlanRegressionsApi.md#gettestplanregressioncount) | **GET** /testplanregressions/count | Get test plan regressions\&#39; count |
| [**getTestPlanRegressions**](TestPlanRegressionsApi.md#gettestplanregressions) | **GET** /testplanregressions | Get test plan regressions |
| [**updateTestPlanRegression**](TestPlanRegressionsApi.md#updatetestplanregression) | **PUT** /testplanregressions/{id} | Updates a test plan regression |



## addTestPlanRegression

> TestPlanRegression addTestPlanRegression(testPlanRegressionPayload)

Add a test plan regression

Adds a new regression for a test plan

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { AddTestPlanRegressionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // TestPlanRegressionPayload | Config to add (optional)
    testPlanRegressionPayload: ...,
  } satisfies AddTestPlanRegressionRequest;

  try {
    const data = await api.addTestPlanRegression(body);
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
| **testPlanRegressionPayload** | [TestPlanRegressionPayload](TestPlanRegressionPayload.md) | Config to add | [Optional] |

### Return type

[**TestPlanRegression**](TestPlanRegression.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created TestPlanRegression |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestPlanRegression

> object deleteTestPlanRegression(id)

Deletes test plan regression

Deletes a specific test plan regression

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { DeleteTestPlanRegressionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // number | Test Plan Regression ID
    id: 8.14,
  } satisfies DeleteTestPlanRegressionRequest;

  try {
    const data = await api.deleteTestPlanRegression(body);
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
| **id** | `number` | Test Plan Regression ID | [Defaults to `undefined`] |

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
| **200** | Test Plan Regression deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanRegression

> TestPlanRegression getTestPlanRegression(id)

Get test plan regression

Get details of specific test plan regression

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { GetTestPlanRegressionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // number | Test Plan Regression ID
    id: 8.14,
  } satisfies GetTestPlanRegressionRequest;

  try {
    const data = await api.getTestPlanRegression(body);
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
| **id** | `number` | Test Plan Regression ID | [Defaults to `undefined`] |

### Return type

[**TestPlanRegression**](TestPlanRegression.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test plan regression |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanRegressionCount

> Count getTestPlanRegressionCount(project)

Get test plan regressions\&#39; count

Get test plan regressions\&#39; count for a specific project

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { GetTestPlanRegressionCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetTestPlanRegressionCountRequest;

  try {
    const data = await api.getTestPlanRegressionCount(body);
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

### Return type

[**Count**](Count.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of test plan regressions |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanRegressions

> Array&lt;TestPlanRegression&gt; getTestPlanRegressions(project, testplan, testPlanConfigurationId, limit, start, sort, filter)

Get test plan regressions

Get details of regressions for specific test plan

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { GetTestPlanRegressionsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Test Plan ID
    testplan: 1,
    // number | Test Plan Configuration ID (optional)
    testPlanConfigurationId: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestPlanRegressionsRequest;

  try {
    const data = await api.getTestPlanRegressions(body);
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
| **testPlanConfigurationId** | `number` | Test Plan Configuration ID | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestPlanRegression&gt;**](TestPlanRegression.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | list of regressions |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestPlanRegression

> TestPlanRegression updateTestPlanRegression(id, testPlanRegressionPayload)

Updates a test plan regression

Test Plan Regression to update

### Example

```ts
import {
  Configuration,
  TestPlanRegressionsApi,
} from '@testcollab/sdk';
import type { UpdateTestPlanRegressionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanRegressionsApi(config);

  const body = {
    // number | Test Plan Regression ID
    id: 8.14,
    // TestPlanRegressionPayload (optional)
    testPlanRegressionPayload: ...,
  } satisfies UpdateTestPlanRegressionRequest;

  try {
    const data = await api.updateTestPlanRegression(body);
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
| **id** | `number` | Test Plan Regression ID | [Defaults to `undefined`] |
| **testPlanRegressionPayload** | [TestPlanRegressionPayload](TestPlanRegressionPayload.md) |  | [Optional] |

### Return type

[**TestPlanRegression**](TestPlanRegression.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Plan Regression |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

