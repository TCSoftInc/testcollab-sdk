# RequirementFoldersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**copyRequirementFolder**](RequirementFoldersApi.md#copyrequirementfolder) | **POST** /requirementfolders/copy | Duplicate requirement folder |
| [**createRequirementFolder**](RequirementFoldersApi.md#createrequirementfolder) | **POST** /requirementfolders | Create a new requirement folder |
| [**deleteRequirementFolder**](RequirementFoldersApi.md#deleterequirementfolder) | **DELETE** /requirementfolders/{id} | Delete requirement folder |
| [**getRequirementFolder**](RequirementFoldersApi.md#getrequirementfolder) | **GET** /requirementfolders/{id} | Get requirement folder |
| [**getRequirementFolderCount**](RequirementFoldersApi.md#getrequirementfoldercount) | **GET** /requirementfolders/count | Get requirement folders\&#39; count |
| [**getRequirementFolderTree**](RequirementFoldersApi.md#getrequirementfoldertree) | **GET** /requirementfolders/getTree | Get requirement folder tree |
| [**getRequirementFolders**](RequirementFoldersApi.md#getrequirementfolders) | **GET** /requirementfolders | Get requirement folders |
| [**setRequirementsOrder**](RequirementFoldersApi.md#setrequirementsorder) | **POST** /requirementfolders/setOrder | Set sort order for requirement folders |
| [**updateRequirementFolder**](RequirementFoldersApi.md#updaterequirementfolder) | **PUT** /requirementfolders/{id} | Updates a requirement folder |



## copyRequirementFolder

> BulkActionResult copyRequirementFolder(project, requirementFolderCopyPayload)

Duplicate requirement folder

Duplicates a requirement folder

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { CopyRequirementFolderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // RequirementFolderCopyPayload | Requirement folder to be duplicated (optional)
    requirementFolderCopyPayload: ...,
  } satisfies CopyRequirementFolderRequest;

  try {
    const data = await api.copyRequirementFolder(body);
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
| **requirementFolderCopyPayload** | [RequirementFolderCopyPayload](RequirementFolderCopyPayload.md) | Requirement folder to be duplicated | [Optional] |

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


## createRequirementFolder

> GenericFolder createRequirementFolder(genericFolderPayload)

Create a new requirement folder

Requirement Folder to add

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { CreateRequirementFolderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // GenericFolderPayload (optional)
    genericFolderPayload: ...,
  } satisfies CreateRequirementFolderRequest;

  try {
    const data = await api.createRequirementFolder(body);
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
| **genericFolderPayload** | [GenericFolderPayload](GenericFolderPayload.md) |  | [Optional] |

### Return type

[**GenericFolder**](GenericFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Requirement Folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteRequirementFolder

> GenericActionResult deleteRequirementFolder(id)

Delete requirement folder

Deletes a specific requirement folder

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { DeleteRequirementFolderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Requirement Folder ID
    id: 8.14,
  } satisfies DeleteRequirementFolderRequest;

  try {
    const data = await api.deleteRequirementFolder(body);
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
| **id** | `number` | Requirement Folder ID | [Defaults to `undefined`] |

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
| **200** | Requirement Folder deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRequirementFolder

> GenericFolder getRequirementFolder(id)

Get requirement folder

Get details of specific requirement folder

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { GetRequirementFolderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Requirement Folder ID
    id: 8.14,
  } satisfies GetRequirementFolderRequest;

  try {
    const data = await api.getRequirementFolder(body);
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
| **id** | `number` | Requirement Folder ID | [Defaults to `undefined`] |

### Return type

[**GenericFolder**](GenericFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected requirement folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRequirementFolderCount

> Count getRequirementFolderCount(project)

Get requirement folders\&#39; count

Get requirement folders\&#39; count in a specific project

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { GetRequirementFolderCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetRequirementFolderCountRequest;

  try {
    const data = await api.getRequirementFolderCount(body);
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
| **200** | Count of requirement folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRequirementFolderTree

> Array&lt;GenericFolderTree&gt; getRequirementFolderTree(project)

Get requirement folder tree

Get requirement folder tree for a specific project

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { GetRequirementFolderTreeRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Project ID
    project: 56,
  } satisfies GetRequirementFolderTreeRequest;

  try {
    const data = await api.getRequirementFolderTree(body);
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

[**Array&lt;GenericFolderTree&gt;**](GenericFolderTree.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of requirement folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRequirementFolders

> Array&lt;GenericFolder&gt; getRequirementFolders(project, limit, sort, start, filter)

Get requirement folders

Get list of requirement folders for a specific project

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { GetRequirementFoldersRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

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
  } satisfies GetRequirementFoldersRequest;

  try {
    const data = await api.getRequirementFolders(body);
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

[**Array&lt;GenericFolder&gt;**](GenericFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of requirement folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setRequirementsOrder

> CreateActionResult setRequirementsOrder(genericFoldersOrderPayload)

Set sort order for requirement folders

Set sort order for requirement folders

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { SetRequirementsOrderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // GenericFoldersOrderPayload | Sort order details (optional)
    genericFoldersOrderPayload: ...,
  } satisfies SetRequirementsOrderRequest;

  try {
    const data = await api.setRequirementsOrder(body);
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
| **genericFoldersOrderPayload** | [GenericFoldersOrderPayload](GenericFoldersOrderPayload.md) | Sort order details | [Optional] |

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


## updateRequirementFolder

> GenericFolder updateRequirementFolder(id, genericFolderPayload)

Updates a requirement folder

Requirement Folder to update

### Example

```ts
import {
  Configuration,
  RequirementFoldersApi,
} from 'testcollab-sdk';
import type { UpdateRequirementFolderRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new RequirementFoldersApi(config);

  const body = {
    // number | Requirement Folder ID
    id: 8.14,
    // GenericFolderPayload (optional)
    genericFolderPayload: ...,
  } satisfies UpdateRequirementFolderRequest;

  try {
    const data = await api.updateRequirementFolder(body);
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
| **id** | `number` | Requirement Folder ID | [Defaults to `undefined`] |
| **genericFolderPayload** | [GenericFolderPayload](GenericFolderPayload.md) |  | [Optional] |

### Return type

[**GenericFolder**](GenericFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Requirement Folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

