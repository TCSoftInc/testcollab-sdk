# ReleasesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addRelease**](ReleasesApi.md#addrelease) | **POST** /releases | Create a release |
| [**countReleases**](ReleasesApi.md#countreleases) | **GET** /releases/count | Count releases |
| [**deleteRelease**](ReleasesApi.md#deleterelease) | **DELETE** /releases/{id} | Delete a release |
| [**editRelease**](ReleasesApi.md#editrelease) | **PUT** /releases/{id} | Edit a release |
| [**getRelease**](ReleasesApi.md#getrelease) | **GET** /releases/{id} | Get release |
| [**getReleaseReadiness**](ReleasesApi.md#getreleasereadiness) | **GET** /releases/{id}/readiness | Get release readiness dashboard data |
| [**getReleaseReadinessByToken**](ReleasesApi.md#getreleasereadinessbytoken) | **GET** /releases/readiness/{token} | Get release readiness by public token |
| [**getReleases**](ReleasesApi.md#getreleases) | **GET** /releases | Get releases |



## addRelease

> ReleaseMinified addRelease(releasePayload)

Create a release

Creates a new release

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { AddReleaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // ReleasePayload | Release to create (optional)
    releasePayload: ...,
  } satisfies AddReleaseRequest;

  try {
    const data = await api.addRelease(body);
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
| **releasePayload** | [ReleasePayload](ReleasePayload.md) | Release to create | [Optional] |

### Return type

[**ReleaseMinified**](ReleaseMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created release |  -  |
| **400** | Bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## countReleases

> Count countReleases(project, status)

Count releases

Get count of releases for a specific project

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { CountReleasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // 'planned' | 'in_progress' | 'ready' | 'shipped' | 'blocked' | Filter by release status (optional)
    status: status_example,
  } satisfies CountReleasesRequest;

  try {
    const data = await api.countReleases(body);
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
| **status** | `planned`, `in_progress`, `ready`, `shipped`, `blocked` | Filter by release status | [Optional] [Defaults to `undefined`] [Enum: planned, in_progress, ready, shipped, blocked] |

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
| **200** | Count of releases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteRelease

> object deleteRelease(id, project)

Delete a release

Deletes a specific release. Does not delete associated test plans.

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { DeleteReleaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Release ID
    id: 1,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteReleaseRequest;

  try {
    const data = await api.deleteRelease(body);
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
| **id** | `number` | Release ID | [Defaults to `undefined`] |
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
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## editRelease

> ReleaseMinified editRelease(id, releasePayload)

Edit a release

Edits a specific release

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { EditReleaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Release ID
    id: 1,
    // ReleasePayload | Updated release data (optional)
    releasePayload: ...,
  } satisfies EditReleaseRequest;

  try {
    const data = await api.editRelease(body);
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
| **id** | `number` | Release ID | [Defaults to `undefined`] |
| **releasePayload** | [ReleasePayload](ReleasePayload.md) | Updated release data | [Optional] |

### Return type

[**ReleaseMinified**](ReleaseMinified.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated release |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRelease

> Release getRelease(id)

Get release

Get details of a specific release

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { GetReleaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Release ID
    id: 1,
  } satisfies GetReleaseRequest;

  try {
    const data = await api.getRelease(body);
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
| **id** | `number` | Release ID | [Defaults to `undefined`] |

### Return type

[**Release**](Release.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReleaseReadiness

> ReleaseReadiness getReleaseReadiness(id)

Get release readiness dashboard data

Returns aggregated readiness data for a release including execution summary, open defects, coverage by suite, evidence metrics, comparison to previous release, and a computed Go/No-Go verdict. Uses the latest run (regression) of each test plan in the release. 

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { GetReleaseReadinessRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Release ID
    id: 1,
  } satisfies GetReleaseReadinessRequest;

  try {
    const data = await api.getReleaseReadiness(body);
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
| **id** | `number` | Release ID | [Defaults to `undefined`] |

### Return type

[**ReleaseReadiness**](ReleaseReadiness.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release readiness dashboard data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReleaseReadinessByToken

> ReleaseReadiness getReleaseReadinessByToken(token)

Get release readiness by public token

Public endpoint (no authentication required). Returns the same readiness data as the authenticated endpoint, looked up by the release\&#39;s public_token. Only works if is_public is true on the release. 

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { GetReleaseReadinessByTokenRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const api = new ReleasesApi();

  const body = {
    // string | Public sharing token for the release
    token: a1b2c3d4-e5f6-7890-abcd-ef1234567890,
  } satisfies GetReleaseReadinessByTokenRequest;

  try {
    const data = await api.getReleaseReadinessByToken(body);
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
| **token** | `string` | Public sharing token for the release | [Defaults to `undefined`] |

### Return type

[**ReleaseReadiness**](ReleaseReadiness.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release readiness dashboard data |  -  |
| **404** | Not found — invalid token or release not public |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReleases

> Array&lt;Release&gt; getReleases(project, limit, start, sort, filter, status)

Get releases

Get releases for a specific project

### Example

```ts
import {
  Configuration,
  ReleasesApi,
} from '@testcollab/sdk';
import type { GetReleasesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReleasesApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object (optional)
    filter: filter_example,
    // 'planned' | 'in_progress' | 'ready' | 'shipped' | 'blocked' | Filter by release status (optional)
    status: status_example,
  } satisfies GetReleasesRequest;

  try {
    const data = await api.getReleases(body);
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
| **filter** | `string` | Stringified filter object | [Optional] [Defaults to `undefined`] |
| **status** | `planned`, `in_progress`, `ready`, `shipped`, `blocked` | Filter by release status | [Optional] [Defaults to `undefined`] [Enum: planned, in_progress, ready, shipped, blocked] |

### Return type

[**Array&lt;Release&gt;**](Release.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of releases |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

