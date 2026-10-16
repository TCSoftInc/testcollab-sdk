# TrashApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**emptyTrash**](TrashApi.md#emptytrash) | **POST** /trashitems/empty | Empty a project\&#39;s Trash permanently |
| [**getTrashItems**](TrashApi.md#gettrashitems) | **GET** /trashitems | List a project\&#39;s Trash |
| [**getTrashItemsCount**](TrashApi.md#gettrashitemscount) | **GET** /trashitems/count | Count a project\&#39;s Trash entries |
| [**restoreTrashItem**](TrashApi.md#restoretrashitem) | **POST** /trashitems/{id}/restore | Restore an item from Trash |
| [**restoreTrashItems**](TrashApi.md#restoretrashitems) | **POST** /trashitems/bulkRestore | Restore multiple items from Trash in one queue |



## emptyTrash

> TrashActionResult emptyTrash(emptyTrashPayload, project)

Empty a project\&#39;s Trash permanently

Company Administrators only; all plans. Requires an exact EMPTY TRASH confirmation and queues permanent removal of all entries in this project\&#39;s Trash at request acceptance, including expired entries not yet removed by the daily job. Items deleted after acceptance are not part of this request. Descendants and linked copies retained with an entry are removed with it. This operation cannot be undone. Concurrent restore and purge operations must claim entries exclusively; an item already restored is not removed. The activity log records both the empty request and each final removal.

### Example

```ts
import {
  Configuration,
  TrashApi,
} from '@testcollab/sdk';
import type { EmptyTrashRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TrashApi(config);

  const body = {
    // EmptyTrashPayload
    emptyTrashPayload: ...,
    // number | Project whose Trash will be emptied.
    project: 56,
  } satisfies EmptyTrashRequest;

  try {
    const data = await api.emptyTrash(body);
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
| **emptyTrashPayload** | [EmptyTrashPayload](EmptyTrashPayload.md) |  | |
| **project** | `number` | Project whose Trash will be emptied. | [Defaults to `undefined`] |

### Return type

[**TrashActionResult**](TrashActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Empty Trash accepted. Poll the queue for completion or failure. |  -  |
| **400** | Invalid project or missing or incorrect confirmation. |  -  |
| **401** | Authentication required. |  -  |
| **403** | Company Administrator access to the requested project is required. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTrashItems

> Array&lt;TrashItem&gt; getTrashItems(project, start, limit)

List a project\&#39;s Trash

Available on all plans to company Administrators only, with access checked in the company that owns the requested project. Project roles and test case delete permissions do not grant Trash access. Lists items still within their 60-day restore period, newest deletion first, then highest Trash entry ID. A suite entry includes the sub-suites and cases moved to Trash with it; those children are not listed separately. Items deleted separately before their parent suite keep their own entries and original expiry times. Linked copies moved with their source are restored with that source, rather than listed as separate entries in destination projects.

### Example

```ts
import {
  Configuration,
  TrashApi,
} from '@testcollab/sdk';
import type { GetTrashItemsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TrashApi(config);

  const body = {
    // number | Project ID.
    project: 56,
    // number | Number of entries to skip. (optional)
    start: 56,
    // number | Maximum entries to return. Unbounded reads are not supported. (optional)
    limit: 56,
  } satisfies GetTrashItemsRequest;

  try {
    const data = await api.getTrashItems(body);
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
| **project** | `number` | Project ID. | [Defaults to `undefined`] |
| **start** | `number` | Number of entries to skip. | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum entries to return. Unbounded reads are not supported. | [Optional] [Defaults to `25`] |

### Return type

[**Array&lt;TrashItem&gt;**](TrashItem.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Trash entries for this project. |  -  |
| **400** | Invalid project or pagination parameters. |  -  |
| **401** | Authentication required. |  -  |
| **403** | Company Administrator access to the requested project is required. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTrashItemsCount

> Count getTrashItemsCount(project)

Count a project\&#39;s Trash entries

Counts entries returned by GET /trashitems before pagination, using the same 60-day deadline and suite grouping. Company Administrators only; all plans.

### Example

```ts
import {
  Configuration,
  TrashApi,
} from '@testcollab/sdk';
import type { GetTrashItemsCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TrashApi(config);

  const body = {
    // number | Project ID.
    project: 56,
  } satisfies GetTrashItemsCountRequest;

  try {
    const data = await api.getTrashItemsCount(body);
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
| **project** | `number` | Project ID. | [Defaults to `undefined`] |

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
| **200** | Number of restorable Trash entries. |  -  |
| **400** | Invalid project. |  -  |
| **401** | Authentication required. |  -  |
| **403** | Company Administrator access to the requested project is required. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## restoreTrashItem

> TrashActionResult restoreTrashItem(project, id)

Restore an item from Trash

Company Administrators only; all plans. Queues restoration of the entry to its original location, preserving IDs, archive state, revisions, test plan results, comments, attachments, tags, requirement links and linked copies. Restoring a suite also restores the descendants deleted with that suite, but does not restore entries deleted separately before it. Restore a separately trashed parent first; a missing parent or conflicting active suite name prevents restoration. The original project and any linked-copy destination must still exist. The deadline and dependencies are checked again in the worker. An entry being restored or permanently removed cannot be claimed by another operation. The queue reports failure if a dependency changes or the deadline passes before the worker claims the entry; it must not report a partial restore as success.

### Example

```ts
import {
  Configuration,
  TrashApi,
} from '@testcollab/sdk';
import type { RestoreTrashItemRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TrashApi(config);

  const body = {
    // number | Project that owns the Trash entry.
    project: 56,
    // number | Trash entry ID from GET /trashitems, not the original resource ID.
    id: 56,
  } satisfies RestoreTrashItemRequest;

  try {
    const data = await api.restoreTrashItem(body);
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
| **project** | `number` | Project that owns the Trash entry. | [Defaults to `undefined`] |
| **id** | `number` | Trash entry ID from GET /trashitems, not the original resource ID. | [Defaults to `undefined`] |

### Return type

[**TrashActionResult**](TrashActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Restore accepted. Poll the queue before refreshing active lists. |  -  |
| **400** | Invalid parameters. |  -  |
| **401** | Authentication required. |  -  |
| **403** | Company Administrator access to the requested project is required. |  -  |
| **404** | No Trash entry with this ID in the requested project. |  -  |
| **409** | Restore dependency conflict or another operation already owns the entry. |  -  |
| **410** | The 60-day restore period has expired. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## restoreTrashItems

> TrashActionResult restoreTrashItems(trashBulkRestorePayload, project)

Restore multiple items from Trash in one queue

Company Administrators only; all plans. Validates the selected entries and creates one restore queue containing every Trash entry ID. The worker restores parent suites before child suites and restores test cases after suites so dependencies selected in the same request are available. The existing single-item restore operation is unchanged. Poll the returned queue for the overall result.

### Example

```ts
import {
  Configuration,
  TrashApi,
} from '@testcollab/sdk';
import type { RestoreTrashItemsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TrashApi(config);

  const body = {
    // TrashBulkRestorePayload
    trashBulkRestorePayload: ...,
    // number | Project that owns every selected Trash entry.
    project: 56,
  } satisfies RestoreTrashItemsRequest;

  try {
    const data = await api.restoreTrashItems(body);
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
| **trashBulkRestorePayload** | [TrashBulkRestorePayload](TrashBulkRestorePayload.md) |  | |
| **project** | `number` | Project that owns every selected Trash entry. | [Defaults to `undefined`] |

### Return type

[**TrashActionResult**](TrashActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk restore accepted as one queued operation. |  -  |
| **400** | Invalid or empty entry selection. |  -  |
| **401** | Authentication required. |  -  |
| **403** | Company Administrator access to the requested project is required. |  -  |
| **404** | One or more selected entries are unavailable or belong to another project. |  -  |
| **409** | One or more selected entries reached the retention deadline. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

