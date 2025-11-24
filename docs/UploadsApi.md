# UploadsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createUpload**](UploadsApi.md#createupload) | **POST** /upload | Create an upload |
| [**deleteUpload**](UploadsApi.md#deleteupload) | **DELETE** /upload/files/{id} | Delete an upload |
| [**getAttachment**](UploadsApi.md#getattachment) | **GET** /companies/getAttachment | Get specific uploaded data |
| [**getUpload**](UploadsApi.md#getupload) | **GET** /upload/files/{id} | Get upload |
| [**getUploadCount**](UploadsApi.md#getuploadcount) | **GET** /upload/files/count | Get uploads\&#39; count |
| [**getUploads**](UploadsApi.md#getuploads) | **GET** /upload/files | Get list of uploads |
| [**updateUpload**](UploadsApi.md#updateupload) | **PUT** /upload/files/{id} | Update an upload |



## createUpload

> Array&lt;Upload&gt; createUpload(files, company)

Create an upload

Creates a new upload

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { CreateUploadRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // Blob
    files: BINARY_DATA_HERE,
    // number | Company ID
    company: 8.14,
  } satisfies CreateUploadRequest;

  try {
    const data = await api.createUpload(body);
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
| **files** | `Blob` |  | [Defaults to `undefined`] |
| **company** | `number` | Company ID | [Defaults to `undefined`] |

### Return type

[**Array&lt;Upload&gt;**](Upload.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Upload |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteUpload

> object deleteUpload(id)

Delete an upload

Deletes a specific uploaded file

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { DeleteUploadRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // number | Upload ID
    id: 8.14,
  } satisfies DeleteUploadRequest;

  try {
    const data = await api.deleteUpload(body);
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
| **id** | `number` | Upload ID | [Defaults to `undefined`] |

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
| **200** | Upload deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAttachment

> Upload getAttachment(company, id, authToken)

Get specific uploaded data

Get details of a specific file uploaded as attachment for a company

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { GetAttachmentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const api = new UploadsApi();

  const body = {
    // number | Company ID
    company: 8.14,
    // number | Attachment ID
    id: 8.14,
    // string | jwt token (optional)
    authToken: authToken_example,
  } satisfies GetAttachmentRequest;

  try {
    const data = await api.getAttachment(body);
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
| **id** | `number` | Attachment ID | [Defaults to `undefined`] |
| **authToken** | `string` | jwt token | [Optional] [Defaults to `undefined`] |

### Return type

[**Upload**](Upload.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected upload |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUpload

> Upload getUpload(id)

Get upload

Get details of an uploaded file

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { GetUploadRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // number | Upload ID
    id: 8.14,
  } satisfies GetUploadRequest;

  try {
    const data = await api.getUpload(body);
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
| **id** | `number` | Upload ID | [Defaults to `undefined`] |

### Return type

[**Upload**](Upload.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected upload |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUploadCount

> Count getUploadCount(project)

Get uploads\&#39; count

Get uploads\&#39; count for a specific project

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { GetUploadCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetUploadCountRequest;

  try {
    const data = await api.getUploadCount(body);
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
| **200** | Count of uploads |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUploads

> Array&lt;Upload&gt; getUploads(company, limit, sort, start, filter)

Get list of uploads

Get list of files uploaded for a company

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { GetUploadsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // number | Company ID
    company: 1,
    // number | Maximum number of records (optional)
    limit: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetUploadsRequest;

  try {
    const data = await api.getUploads(body);
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
| **limit** | `number` | Maximum number of records | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Upload&gt;**](Upload.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of uploads |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateUpload

> Upload updateUpload(id, uploadPayload)

Update an upload

Updates an upload

### Example

```ts
import {
  Configuration,
  UploadsApi,
} from '@testcollab/sdk';
import type { UpdateUploadRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UploadsApi(config);

  const body = {
    // number | Upload ID
    id: 8.14,
    // UploadPayload (optional)
    uploadPayload: ...,
  } satisfies UpdateUploadRequest;

  try {
    const data = await api.updateUpload(body);
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
| **id** | `number` | Upload ID | [Defaults to `undefined`] |
| **uploadPayload** | [UploadPayload](UploadPayload.md) |  | [Optional] |

### Return type

[**Upload**](Upload.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Upload |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

