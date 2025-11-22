# CustomFieldsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCustomField**](CustomFieldsApi.md#createcustomfield) | **POST** /customfields | Create a new custom field |
| [**deleteCustomField**](CustomFieldsApi.md#deletecustomfield) | **DELETE** /customfields/{id} | Deletes given custom field |
| [**getCustomField**](CustomFieldsApi.md#getcustomfield) | **GET** /customfields/{id} | Get custom fields |
| [**getCustomFieldCount**](CustomFieldsApi.md#getcustomfieldcount) | **GET** /customfields/count | Get custom fields count |
| [**getCustomFields**](CustomFieldsApi.md#getcustomfields) | **GET** /customfields | Get list of custom fields |
| [**setCustomFieldsSortOrder**](CustomFieldsApi.md#setcustomfieldssortorder) | **POST** /customfields/setSortOrder | Set sort order for custom fields |
| [**updateCustomField**](CustomFieldsApi.md#updatecustomfield) | **PUT** /customfields/{id} | Updates a custom field |



## createCustomField

> CustomField createCustomField(customFieldPayload)

Create a new custom field

Custom Field to add

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { CreateCustomFieldRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // CustomFieldPayload (optional)
    customFieldPayload: ...,
  } satisfies CreateCustomFieldRequest;

  try {
    const data = await api.createCustomField(body);
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
| **customFieldPayload** | [CustomFieldPayload](CustomFieldPayload.md) |  | [Optional] |

### Return type

[**CustomField**](CustomField.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Custom Field |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteCustomField

> object deleteCustomField(id)

Deletes given custom field

Deletes specific custom field

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { DeleteCustomFieldRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // number | Custom Field ID
    id: 8.14,
  } satisfies DeleteCustomFieldRequest;

  try {
    const data = await api.deleteCustomField(body);
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
| **id** | `number` | Custom Field ID | [Defaults to `undefined`] |

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
| **200** | Custom Field deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCustomField

> CustomField getCustomField(id)

Get custom fields

Get custom fields

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { GetCustomFieldRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // number | Custom Field ID
    id: 8.14,
  } satisfies GetCustomFieldRequest;

  try {
    const data = await api.getCustomField(body);
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
| **id** | `number` | Custom Field ID | [Defaults to `undefined`] |

### Return type

[**CustomField**](CustomField.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected custom field |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCustomFieldCount

> Count getCustomFieldCount(company)

Get custom fields count

Get custom fields count

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { GetCustomFieldCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // number | Company ID
    company: 1,
  } satisfies GetCustomFieldCountRequest;

  try {
    const data = await api.getCustomFieldCount(body);
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
| **company** | `number` | Company ID | [Defaults to `undefined`] |

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
| **200** | Count of custom fields |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCustomFields

> Array&lt;CustomField&gt; getCustomFields(company, limit, start, sort, filter)

Get list of custom fields

Get company specific list of custom fields

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { GetCustomFieldsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // number | Company ID
    company: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetCustomFieldsRequest;

  try {
    const data = await api.getCustomFields(body);
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
| **company** | `number` | Company ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;CustomField&gt;**](CustomField.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of custom fields |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setCustomFieldsSortOrder

> CreateActionResult setCustomFieldsSortOrder(customFieldsSortOrderPayload)

Set sort order for custom fields

Set sort order for custom fields

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { SetCustomFieldsSortOrderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // CustomFieldsSortOrderPayload | New sort order details (optional)
    customFieldsSortOrderPayload: ...,
  } satisfies SetCustomFieldsSortOrderRequest;

  try {
    const data = await api.setCustomFieldsSortOrder(body);
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
| **customFieldsSortOrderPayload** | [CustomFieldsSortOrderPayload](CustomFieldsSortOrderPayload.md) | New sort order details | [Optional] |

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


## updateCustomField

> CustomField updateCustomField(id, customFieldPayload)

Updates a custom field

Custom Field to update

### Example

```ts
import {
  Configuration,
  CustomFieldsApi,
} from 'testcollab-sdk';
import type { UpdateCustomFieldRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomFieldsApi(config);

  const body = {
    // number | Custom Field ID
    id: 8.14,
    // CustomFieldPayload (optional)
    customFieldPayload: ...,
  } satisfies UpdateCustomFieldRequest;

  try {
    const data = await api.updateCustomField(body);
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
| **id** | `number` | Custom Field ID | [Defaults to `undefined`] |
| **customFieldPayload** | [CustomFieldPayload](CustomFieldPayload.md) |  | [Optional] |

### Return type

[**CustomField**](CustomField.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Custom Field |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

