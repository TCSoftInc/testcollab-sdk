# SuitesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addSuite**](SuitesApi.md#addsuite) | **POST** /suites | Add test suite |
| [**copySuite**](SuitesApi.md#copysuite) | **POST** /suites/copy | Duplicate suite |
| [**deleteSuite**](SuitesApi.md#deletesuite) | **DELETE** /suites/{id} | Delete suite |
| [**getAllSuites**](SuitesApi.md#getallsuites) | **GET** /suites | Get all suites |
| [**getProjectSuitesTree**](SuitesApi.md#getprojectsuitestree) | **GET** /projectsuitetrees | Get suite tree for a given project |
| [**getSuite**](SuitesApi.md#getsuite) | **GET** /suites/{id} | Get specific suite |
| [**linkSuite**](SuitesApi.md#linksuite) | **POST** /suites/link | Link suite |
| [**setSuitesOrder**](SuitesApi.md#setsuitesorder) | **POST** /suites/setOrder | Set sort order for suites |
| [**suitesBulkAction**](SuitesApi.md#suitesbulkaction) | **POST** /suites/bulkAction | Bulk actions for suites |
| [**unlinkSuite**](SuitesApi.md#unlinksuite) | **POST** /suites/unlink | Unlink suite |
| [**updateSuite**](SuitesApi.md#updatesuite) | **PUT** /suites/{id} | Updates a suite |



## addSuite

> Suite addSuite(addSuitePayload)

Add test suite

Add a test suite

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { AddSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // AddSuitePayload (optional)
    addSuitePayload: ...,
  } satisfies AddSuiteRequest;

  try {
    const data = await api.addSuite(body);
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
| **addSuitePayload** | [AddSuitePayload](AddSuitePayload.md) |  | [Optional] |

### Return type

[**Suite**](Suite.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## copySuite

> BulkActionResult copySuite(project, suiteCopyPayload)

Duplicate suite

Duplicates a specific suite

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { CopySuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // SuiteCopyPayload | Suite to be duplicated (optional)
    suiteCopyPayload: ...,
  } satisfies CopySuiteRequest;

  try {
    const data = await api.copySuite(body);
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
| **suiteCopyPayload** | [SuiteCopyPayload](SuiteCopyPayload.md) | Suite to be duplicated | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

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


## deleteSuite

> object deleteSuite(project, id)

Delete suite

Deletes a specific suite

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { DeleteSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Suite ID
    id: 8.14,
  } satisfies DeleteSuiteRequest;

  try {
    const data = await api.deleteSuite(body);
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
| **id** | `number` | Suite ID | [Defaults to `undefined`] |

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
| **200** | Suite deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAllSuites

> Array&lt;Suite&gt; getAllSuites(project, filter)

Get all suites

fetch suite data

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { GetAllSuitesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetAllSuitesRequest;

  try {
    const data = await api.getAllSuites(body);
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
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Suite&gt;**](Suite.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected suite |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectSuitesTree

> Array&lt;ProjectSuiteTree&gt; getProjectSuitesTree(project)

Get suite tree for a given project

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { GetProjectSuitesTreeRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 1,
  } satisfies GetProjectSuitesTreeRequest;

  try {
    const data = await api.getProjectSuitesTree(body);
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

[**Array&lt;ProjectSuiteTree&gt;**](ProjectSuiteTree.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Suite tree for this project, this will always be an array with one element only. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSuite

> Suite getSuite(project, id)

Get specific suite

fetch suite data

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { GetSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Suite ID
    id: 8.14,
  } satisfies GetSuiteRequest;

  try {
    const data = await api.getSuite(body);
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
| **id** | `number` | Suite ID | [Defaults to `undefined`] |

### Return type

[**Suite**](Suite.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected suite |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## linkSuite

> BulkActionResult linkSuite(suiteLinkPayload)

Link suite

Creates a suite\&#39;s link

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { LinkSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // SuiteLinkPayload | Create suite link (optional)
    suiteLinkPayload: ...,
  } satisfies LinkSuiteRequest;

  try {
    const data = await api.linkSuite(body);
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
| **suiteLinkPayload** | [SuiteLinkPayload](SuiteLinkPayload.md) | Create suite link | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

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


## setSuitesOrder

> CreateActionResult setSuitesOrder(suitesOrderPayload)

Set sort order for suites

Set sort order for suites

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { SetSuitesOrderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // SuitesOrderPayload | Sort order details (optional)
    suitesOrderPayload: ...,
  } satisfies SetSuitesOrderRequest;

  try {
    const data = await api.setSuitesOrder(body);
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
| **suitesOrderPayload** | [SuitesOrderPayload](SuitesOrderPayload.md) | Sort order details | [Optional] |

### Return type

[**CreateActionResult**](CreateActionResult.md)

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


## suitesBulkAction

> BulkActionResult suitesBulkAction(suitesBulkActionPayload)

Bulk actions for suites

Bulk action for suites

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { SuitesBulkActionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // SuitesBulkActionPayload | Bulk action details (optional)
    suitesBulkActionPayload: ...,
  } satisfies SuitesBulkActionRequest;

  try {
    const data = await api.suitesBulkAction(body);
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
| **suitesBulkActionPayload** | [SuitesBulkActionPayload](SuitesBulkActionPayload.md) | Bulk action details | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

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


## unlinkSuite

> BulkActionResult unlinkSuite(suiteUnlinkPayload)

Unlink suite

Unlinks a specific suite

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { UnlinkSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // SuiteUnlinkPayload | Suite unlink (optional)
    suiteUnlinkPayload: ...,
  } satisfies UnlinkSuiteRequest;

  try {
    const data = await api.unlinkSuite(body);
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
| **suiteUnlinkPayload** | [SuiteUnlinkPayload](SuiteUnlinkPayload.md) | Suite unlink | [Optional] |

### Return type

[**BulkActionResult**](BulkActionResult.md)

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


## updateSuite

> object updateSuite(project, id, addSuitePayload)

Updates a suite

Suite to update

### Example

```ts
import {
  Configuration,
  SuitesApi,
} from '@testcollab/sdk';
import type { UpdateSuiteRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SuitesApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Suite ID
    id: 8.14,
    // AddSuitePayload (optional)
    addSuitePayload: ...,
  } satisfies UpdateSuiteRequest;

  try {
    const data = await api.updateSuite(body);
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
| **id** | `number` | Suite ID | [Defaults to `undefined`] |
| **addSuitePayload** | [AddSuitePayload](AddSuitePayload.md) |  | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Suite Updated |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

