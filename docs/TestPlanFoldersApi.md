# TestPlanFoldersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**copyTestPlanFolder**](TestPlanFoldersApi.md#copytestplanfolder) | **POST** /testplanfolder/copy | Duplicate test plan folder |
| [**createTestPlanFolder**](TestPlanFoldersApi.md#createtestplanfolder) | **POST** /testplanfolders | Create a new test plan folder |
| [**deleteTestPlanFolder**](TestPlanFoldersApi.md#deletetestplanfolder) | **DELETE** /testplanfolders/{id} | Delete test plan folder |
| [**getTestPlanFolder**](TestPlanFoldersApi.md#gettestplanfolder) | **GET** /testplanfolders/{id} | Get test plan folder |
| [**getTestPlanFolderCount**](TestPlanFoldersApi.md#gettestplanfoldercount) | **GET** /testplanfolders/count | Get test plan folders\&#39; count |
| [**getTestPlanFolderTree**](TestPlanFoldersApi.md#gettestplanfoldertree) | **GET** /testplanfolders/getTree | Get test plan folder tree |
| [**getTestPlanFolders**](TestPlanFoldersApi.md#gettestplanfolders) | **GET** /testplanfolders | Get test plan folders |
| [**setTestplansOrder**](TestPlanFoldersApi.md#settestplansorder) | **POST** /testplanfolders/setOrder | Set sort order for testplan folders |
| [**updateTestPlanFolder**](TestPlanFoldersApi.md#updatetestplanfolder) | **PUT** /testplanfolders/{id} | Updates a test plan folder |



## copyTestPlanFolder

> BulkActionResult copyTestPlanFolder(project, testPlanFolderCopyPayload)

Duplicate test plan folder

Duplicates a test plan folder

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { CopyTestPlanFolderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // TestPlanFolderCopyPayload | Test plan folder to be duplicated (optional)
    testPlanFolderCopyPayload: ...,
  } satisfies CopyTestPlanFolderRequest;

  try {
    const data = await api.copyTestPlanFolder(body);
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
| **testPlanFolderCopyPayload** | [TestPlanFolderCopyPayload](TestPlanFolderCopyPayload.md) | Test plan folder to be duplicated | [Optional] |

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


## createTestPlanFolder

> TestPlanFolder createTestPlanFolder(testPlanFolderPayload)

Create a new test plan folder

Test Plan Folder to add

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { CreateTestPlanFolderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // TestPlanFolderPayload (optional)
    testPlanFolderPayload: ...,
  } satisfies CreateTestPlanFolderRequest;

  try {
    const data = await api.createTestPlanFolder(body);
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
| **testPlanFolderPayload** | [TestPlanFolderPayload](TestPlanFolderPayload.md) |  | [Optional] |

### Return type

[**TestPlanFolder**](TestPlanFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Test Plan Folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestPlanFolder

> object deleteTestPlanFolder(id)

Delete test plan folder

Deletes a specific test plan folder

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { DeleteTestPlanFolderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Test Plan Folder ID
    id: 8.14,
  } satisfies DeleteTestPlanFolderRequest;

  try {
    const data = await api.deleteTestPlanFolder(body);
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
| **id** | `number` | Test Plan Folder ID | [Defaults to `undefined`] |

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
| **200** | Test Plan Folder deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanFolder

> TestPlanFolder getTestPlanFolder(id)

Get test plan folder

Get details of specific test plan folder

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { GetTestPlanFolderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Test Plan Folder ID
    id: 8.14,
  } satisfies GetTestPlanFolderRequest;

  try {
    const data = await api.getTestPlanFolder(body);
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
| **id** | `number` | Test Plan Folder ID | [Defaults to `undefined`] |

### Return type

[**TestPlanFolder**](TestPlanFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test plan folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanFolderCount

> Count getTestPlanFolderCount(project)

Get test plan folders\&#39; count

Get test plan folders\&#39; count in a specific project

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { GetTestPlanFolderCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetTestPlanFolderCountRequest;

  try {
    const data = await api.getTestPlanFolderCount(body);
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
| **200** | Count of test plan folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanFolderTree

> Array&lt;FolderTree&gt; getTestPlanFolderTree(project)

Get test plan folder tree

Get test plan folder tree for a specific project

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { GetTestPlanFolderTreeRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Project ID
    project: 56,
  } satisfies GetTestPlanFolderTreeRequest;

  try {
    const data = await api.getTestPlanFolderTree(body);
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

[**Array&lt;FolderTree&gt;**](FolderTree.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test plan folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanFolders

> Array&lt;TestPlanFolder&gt; getTestPlanFolders(project, limit, sort, start, filter)

Get test plan folders

Get list of test plan folders for a specific project

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { GetTestPlanFoldersRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

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
  } satisfies GetTestPlanFoldersRequest;

  try {
    const data = await api.getTestPlanFolders(body);
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

[**Array&lt;TestPlanFolder&gt;**](TestPlanFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of test plan folders |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setTestplansOrder

> CreateActionResult setTestplansOrder(testPlanFoldersOrderPayload)

Set sort order for testplan folders

Set sort order for testplan folders

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { SetTestplansOrderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // TestPlanFoldersOrderPayload | Sort order details (optional)
    testPlanFoldersOrderPayload: ...,
  } satisfies SetTestplansOrderRequest;

  try {
    const data = await api.setTestplansOrder(body);
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
| **testPlanFoldersOrderPayload** | [TestPlanFoldersOrderPayload](TestPlanFoldersOrderPayload.md) | Sort order details | [Optional] |

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


## updateTestPlanFolder

> TestPlanFolder updateTestPlanFolder(id, testPlanFolderPayload)

Updates a test plan folder

Test Plan Folder to update

### Example

```ts
import {
  Configuration,
  TestPlanFoldersApi,
} from '@testcollab/sdk';
import type { UpdateTestPlanFolderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlanFoldersApi(config);

  const body = {
    // number | Test Plan Folder ID
    id: 8.14,
    // TestPlanFolderPayload (optional)
    testPlanFolderPayload: ...,
  } satisfies UpdateTestPlanFolderRequest;

  try {
    const data = await api.updateTestPlanFolder(body);
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
| **id** | `number` | Test Plan Folder ID | [Defaults to `undefined`] |
| **testPlanFolderPayload** | [TestPlanFolderPayload](TestPlanFolderPayload.md) |  | [Optional] |

### Return type

[**TestPlanFolder**](TestPlanFolder.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Plan Folder |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

