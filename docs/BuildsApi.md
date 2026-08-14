# BuildsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addBuild**](BuildsApi.md#addbuild) | **POST** /builds | Create a build |
| [**countBuilds**](BuildsApi.md#countbuilds) | **GET** /builds/count | Count builds |
| [**deleteBuild**](BuildsApi.md#deletebuild) | **DELETE** /builds/{id} | Delete a build |
| [**editBuild**](BuildsApi.md#editbuild) | **PUT** /builds/{id} | Edit a build |
| [**getBuild**](BuildsApi.md#getbuild) | **GET** /builds/{id} | Get build |
| [**getBuildTraceability**](BuildsApi.md#getbuildtraceability) | **GET** /builds/{id}/traceability | Build traceability |
| [**getBuilds**](BuildsApi.md#getbuilds) | **GET** /builds | Get builds |



## addBuild

> BuildMinified addBuild(buildPayload)

Create a build

Creates a new build

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { AddBuildRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // BuildPayload | Build to create (optional)
    buildPayload: ...,
  } satisfies AddBuildRequest;

  try {
    const data = await api.addBuild(body);
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
| **buildPayload** | [BuildPayload](BuildPayload.md) | Build to create | [Optional] |

### Return type

[**BuildMinified**](BuildMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created build |  -  |
| **400** | Bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## countBuilds

> Count countBuilds(project, environment, filter)

Count builds

Get count of builds for a specific project

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { CountBuildsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // string | Filter by exact environment name (optional)
    environment: Production,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies CountBuildsRequest;

  try {
    const data = await api.countBuilds(body);
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
| **environment** | `string` | Filter by exact environment name | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |

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
| **200** | Count of builds |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteBuild

> object deleteBuild(id, project)

Delete a build

Deletes a specific build.

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { DeleteBuildRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Build ID
    id: 1,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteBuildRequest;

  try {
    const data = await api.deleteBuild(body);
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
| **id** | `number` | Build ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

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
| **400** | Build is linked to one or more test plans and cannot be deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## editBuild

> BuildMinified editBuild(id, buildPayload)

Edit a build

Edits a specific build

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { EditBuildRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Build ID
    id: 1,
    // BuildPayload | Updated build data (optional)
    buildPayload: ...,
  } satisfies EditBuildRequest;

  try {
    const data = await api.editBuild(body);
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
| **id** | `number` | Build ID | [Defaults to `undefined`] |
| **buildPayload** | [BuildPayload](BuildPayload.md) | Updated build data | [Optional] |

### Return type

[**BuildMinified**](BuildMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated build |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getBuild

> Build getBuild(id)

Get build

Get details of a specific build

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { GetBuildRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Build ID
    id: 1,
  } satisfies GetBuildRequest;

  try {
    const data = await api.getBuild(body);
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
| **id** | `number` | Build ID | [Defaults to `undefined`] |

### Return type

[**Build**](Build.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Build details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getBuildTraceability

> BuildTraceability getBuildTraceability(id, project)

Build traceability

Aggregated traceability for a build (TCV-6726): execution results summed across every test plan linked to the build, per-plan result distribution, build-scoped risk coverage (risks exercised by test cases executed against the build), and the defects raised against those plans. Powers the Build detail traceability view. The response is provider-neutral — the client chooses the manual vs. Azure DevOps presentation from project settings. 

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { GetBuildTraceabilityRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Build ID
    id: 1,
    // number | Project ID the build belongs to
    project: 1,
  } satisfies GetBuildTraceabilityRequest;

  try {
    const data = await api.getBuildTraceability(body);
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
| **id** | `number` | Build ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID the build belongs to | [Defaults to `undefined`] |

### Return type

[**BuildTraceability**](BuildTraceability.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Build traceability aggregation |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getBuilds

> Array&lt;Build&gt; getBuilds(project, environment, versionContains, limit, start, sort, filter)

Get builds

Get builds for a specific project

### Example

```ts
import {
  Configuration,
  BuildsApi,
} from '@testcollab/sdk';
import type { GetBuildsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new BuildsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // string | Filter by exact environment name (optional)
    environment: Production,
    // string | Case-insensitive search on the version string (optional)
    versionContains: versionContains_example,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object (optional)
    filter: filter_example,
  } satisfies GetBuildsRequest;

  try {
    const data = await api.getBuilds(body);
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
| **environment** | `string` | Filter by exact environment name | [Optional] [Defaults to `undefined`] |
| **versionContains** | `string` | Case-insensitive search on the version string | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Build&gt;**](Build.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of builds |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

