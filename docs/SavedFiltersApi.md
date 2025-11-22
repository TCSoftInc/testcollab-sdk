# SavedFiltersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSavedFilter**](SavedFiltersApi.md#createsavedfilter) | **POST** /savedfilters | Create a new saved filter |
| [**deleteSavedFilter**](SavedFiltersApi.md#deletesavedfilter) | **DELETE** /savedfilters/{id} | Delete saved filter |
| [**getSavedFilter**](SavedFiltersApi.md#getsavedfilter) | **GET** /savedfilters/{id} | Get saved filter |
| [**getSavedFilterCount**](SavedFiltersApi.md#getsavedfiltercount) | **GET** /savedfilters/count | Get saved filters\&#39; count |
| [**getSavedFilters**](SavedFiltersApi.md#getsavedfilters) | **GET** /savedfilters | Get saved filters |
| [**updateSavedFilter**](SavedFiltersApi.md#updatesavedfilter) | **PUT** /savedfilters/{id} | Updates a saved filter |



## createSavedFilter

> SavedFilter createSavedFilter(savedFilterPayload)

Create a new saved filter

Saved Filter to add

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { CreateSavedFilterRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

  const body = {
    // SavedFilterPayload (optional)
    savedFilterPayload: ...,
  } satisfies CreateSavedFilterRequest;

  try {
    const data = await api.createSavedFilter(body);
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
| **savedFilterPayload** | [SavedFilterPayload](SavedFilterPayload.md) |  | [Optional] |

### Return type

[**SavedFilter**](SavedFilter.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Saved Filter |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteSavedFilter

> GenericActionResult deleteSavedFilter(id)

Delete saved filter

Deletes a specific saved filter

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { DeleteSavedFilterRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

  const body = {
    // number | Saved Filter ID
    id: 8.14,
  } satisfies DeleteSavedFilterRequest;

  try {
    const data = await api.deleteSavedFilter(body);
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
| **id** | `number` | Saved Filter ID | [Defaults to `undefined`] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Saved Filter deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSavedFilter

> SavedFilter getSavedFilter(id)

Get saved filter

Get saved filter

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { GetSavedFilterRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

  const body = {
    // number | Saved Filter ID
    id: 8.14,
  } satisfies GetSavedFilterRequest;

  try {
    const data = await api.getSavedFilter(body);
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
| **id** | `number` | Saved Filter ID | [Defaults to `undefined`] |

### Return type

[**SavedFilter**](SavedFilter.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected saved filter |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSavedFilterCount

> Count getSavedFilterCount(project)

Get saved filters\&#39; count

Get saved filters\&#39; count for a specific project

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { GetSavedFilterCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetSavedFilterCountRequest;

  try {
    const data = await api.getSavedFilterCount(body);
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
| **200** | Count of saved filters |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSavedFilters

> Array&lt;SavedFilter&gt; getSavedFilters(project, limit, sort, start, filter)

Get saved filters

Get list of saved filters for a specific project

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { GetSavedFiltersRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

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
  } satisfies GetSavedFiltersRequest;

  try {
    const data = await api.getSavedFilters(body);
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

[**Array&lt;SavedFilter&gt;**](SavedFilter.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of saved filters |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateSavedFilter

> SavedFilter updateSavedFilter(id, savedFilterPayload)

Updates a saved filter

Saved Filter to update

### Example

```ts
import {
  Configuration,
  SavedFiltersApi,
} from 'testcollab-sdk';
import type { UpdateSavedFilterRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SavedFiltersApi(config);

  const body = {
    // number | Saved Filter ID
    id: 8.14,
    // SavedFilterPayload (optional)
    savedFilterPayload: ...,
  } satisfies UpdateSavedFilterRequest;

  try {
    const data = await api.updateSavedFilter(body);
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
| **id** | `number` | Saved Filter ID | [Defaults to `undefined`] |
| **savedFilterPayload** | [SavedFilterPayload](SavedFilterPayload.md) |  | [Optional] |

### Return type

[**SavedFilter**](SavedFilter.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Saved Filter |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

