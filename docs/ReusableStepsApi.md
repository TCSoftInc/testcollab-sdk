# ReusableStepsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteReusableStep**](ReusableStepsApi.md#deletereusablestep) | **DELETE** /reusablesteps/{id} | Delete reusable steps |
| [**getAllReusableSteps**](ReusableStepsApi.md#getallreusablesteps) | **GET** /reusablesteps | Get list of reusable steps |
| [**getReusableStep**](ReusableStepsApi.md#getreusablestep) | **GET** /reusablesteps/{id} | Get reusable step |
| [**getReusablestepsCount**](ReusableStepsApi.md#getreusablestepscount) | **GET** /reusablesteps/count | Get reusable steps\&#39; count |
| [**saveReusableStep**](ReusableStepsApi.md#savereusablestep) | **POST** /reusablesteps | Add reusable steps |
| [**updateReusableStep**](ReusableStepsApi.md#updatereusablestep) | **PUT** /reusablesteps/{id} | Update reusable steps |



## deleteReusableStep

> object deleteReusableStep(project, id)

Delete reusable steps

Deletes a set of reusable steps

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { DeleteReusableStepRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Reusable step ID
    id: 1,
  } satisfies DeleteReusableStepRequest;

  try {
    const data = await api.deleteReusableStep(body);
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
| **id** | `number` | Reusable step ID | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
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


## getAllReusableSteps

> Array&lt;ReusableStep&gt; getAllReusableSteps(project, limit, start, sort, filter)

Get list of reusable steps

Get complete list of reusable steps (with paging)

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { GetAllReusableStepsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetAllReusableStepsRequest;

  try {
    const data = await api.getAllReusableSteps(body);
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
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ReusableStep&gt;**](ReusableStep.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReusableStep

> ReusableStep getReusableStep(project, id)

Get reusable step

Get details of specific reusable step

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { GetReusableStepRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Reusable step ID
    id: 1,
  } satisfies GetReusableStepRequest;

  try {
    const data = await api.getReusableStep(body);
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
| **id** | `number` | Reusable step ID | [Defaults to `undefined`] |

### Return type

[**ReusableStep**](ReusableStep.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
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


## getReusablestepsCount

> Count getReusablestepsCount(project)

Get reusable steps\&#39; count

Get reusable steps\&#39; count

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { GetReusablestepsCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetReusablestepsCountRequest;

  try {
    const data = await api.getReusablestepsCount(body);
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
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of test cases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## saveReusableStep

> ReusableStep saveReusableStep(project, reusableStepPayload)

Add reusable steps

Adds a new set of reusable steps

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { SaveReusableStepRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // ReusableStepPayload | Reusable steps to add (optional)
    reusableStepPayload: ...,
  } satisfies SaveReusableStepRequest;

  try {
    const data = await api.saveReusableStep(body);
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
| **reusableStepPayload** | [ReusableStepPayload](ReusableStepPayload.md) | Reusable steps to add | [Optional] |

### Return type

[**ReusableStep**](ReusableStep.md)

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


## updateReusableStep

> ReusableStep updateReusableStep(id, reusableStepPayload)

Update reusable steps

Updates a set of reusable steps

### Example

```ts
import {
  Configuration,
  ReusableStepsApi,
} from '@testcollab/sdk';
import type { UpdateReusableStepRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReusableStepsApi(config);

  const body = {
    // number | Reusable step ID
    id: 1,
    // ReusableStepPayload | Reusable steps to add (optional)
    reusableStepPayload: ...,
  } satisfies UpdateReusableStepRequest;

  try {
    const data = await api.updateReusableStep(body);
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
| **id** | `number` | Reusable step ID | [Defaults to `undefined`] |
| **reusableStepPayload** | [ReusableStepPayload](ReusableStepPayload.md) | Reusable steps to add | [Optional] |

### Return type

[**ReusableStep**](ReusableStep.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

