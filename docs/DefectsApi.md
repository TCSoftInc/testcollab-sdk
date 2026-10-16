# DefectsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDefect**](DefectsApi.md#createdefect) | **POST** /defects | Create a defect |
| [**deleteDefect**](DefectsApi.md#deletedefect) | **DELETE** /defects/{id} | Deletes a defect |
| [**getDefect**](DefectsApi.md#getdefect) | **GET** /defects/{id} | Get defect |
| [**getDefectCount**](DefectsApi.md#getdefectcount) | **GET** /defects/count | Get count of defects |
| [**getDefects**](DefectsApi.md#getdefects) | **GET** /defects | Get list of defects |
| [**linkDefect**](DefectsApi.md#linkdefect) | **POST** /defects/link | link an existing defect with test case while execution |
| [**unlinkDefect**](DefectsApi.md#unlinkdefect) | **PUT** /defects/{id}/unlink | Unlink a defect from an executed test case |
| [**updateDefect**](DefectsApi.md#updatedefect) | **PUT** /defects/{id} | Updates a defect |



## createDefect

> Defect createDefect(defectPayload)

Create a defect

Create a new defect

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { CreateDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // DefectPayload (optional)
    defectPayload: ...,
  } satisfies CreateDefectRequest;

  try {
    const data = await api.createDefect(body);
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
| **defectPayload** | [DefectPayload](DefectPayload.md) |  | [Optional] |

### Return type

[**Defect**](Defect.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Defect |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteDefect

> object deleteDefect(id)

Deletes a defect

Deletes a specific defect

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { DeleteDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // number | Defect ID
    id: 8.14,
  } satisfies DeleteDefectRequest;

  try {
    const data = await api.deleteDefect(body);
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
| **id** | `number` | Defect ID | [Defaults to `undefined`] |

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
| **200** | Defect deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDefect

> Defect getDefect(id, project)

Get defect

Get details of a reported defect

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { GetDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // number | Defect ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetDefectRequest;

  try {
    const data = await api.getDefect(body);
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
| **id** | `number` | Defect ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**Defect**](Defect.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Get selected defect |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDefectCount

> Count getDefectCount(project, filter)

Get count of defects

Get defects\&#39; count

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { GetDefectCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetDefectCountRequest;

  try {
    const data = await api.getDefectCount(body);
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

[**Count**](Count.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of defects |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDefects

> Array&lt;Defect&gt; getDefects(project, limit, start, sort, filter, testplan)

Get list of defects

Get list of defects

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { GetDefectsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // number | Project ID
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
  } satisfies GetDefectsRequest;

  try {
    const data = await api.getDefects(body);
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
| **testplan** | `number` | Test Plan ID | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Defect&gt;**](Defect.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of defects |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## linkDefect

> Defect linkDefect(linkDefectPayload)

link an existing defect with test case while execution

Link Defect

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { LinkDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // LinkDefectPayload (optional)
    linkDefectPayload: ...,
  } satisfies LinkDefectRequest;

  try {
    const data = await api.linkDefect(body);
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
| **linkDefectPayload** | [LinkDefectPayload](LinkDefectPayload.md) |  | [Optional] |

### Return type

[**Defect**](Defect.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Defect |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## unlinkDefect

> object unlinkDefect(unlinkDefectPayload, id)

Unlink a defect from an executed test case

Requires the project\&#39;s existing manageDefect permission. Removes the selected defect record\&#39;s test case, test plan, execution, plan test case, revision, and step associations. The defect remains in the project\&#39;s defects list, and the underlying external or inbuilt issue is preserved. Other defect records and their associations, execution results, and existing history are unchanged. Records the actor, defect, test case, and test plan in a project activity. The executedtestcase must match the selected defect record\&#39;s current link. Requests for an already unlinked defect fail without adding another activity. 

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { UnlinkDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // UnlinkDefectPayload
    unlinkDefectPayload: ...,
    // number | ID of the TestCollab defect record, not the external issue ID
    id: 56,
  } satisfies UnlinkDefectRequest;

  try {
    const data = await api.unlinkDefect(body);
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
| **unlinkDefectPayload** | [UnlinkDefectPayload](UnlinkDefectPayload.md) |  | |
| **id** | `number` | ID of the TestCollab defect record, not the external issue ID | [Defaults to `undefined`] |

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
| **200** | Defect unlinked and project activity recorded |  -  |
| **400** | Missing or invalid project, defect, or executed test case ID |  -  |
| **401** | Authentication required |  -  |
| **403** | Project access or manageDefect permission denied |  -  |
| **404** | Defect not found in the requested project |  -  |
| **409** | Defect is not linked to the specified executed test case |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateDefect

> Defect updateDefect(id, defectPayload)

Updates a defect

Defect to update

### Example

```ts
import {
  Configuration,
  DefectsApi,
} from '@testcollab/sdk';
import type { UpdateDefectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DefectsApi(config);

  const body = {
    // number | Defect ID
    id: 8.14,
    // DefectPayload (optional)
    defectPayload: ...,
  } satisfies UpdateDefectRequest;

  try {
    const data = await api.updateDefect(body);
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
| **id** | `number` | Defect ID | [Defaults to `undefined`] |
| **defectPayload** | [DefectPayload](DefectPayload.md) |  | [Optional] |

### Return type

[**Defect**](Defect.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Defect |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

