# StatusesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createStatus**](StatusesApi.md#createstatus) | **POST** /statuses | Create a custom status |
| [**deleteStatusById**](StatusesApi.md#deletestatusbyid) | **DELETE** /statuses/{statusId} | Delete a custom status by ID |
| [**getStatusById**](StatusesApi.md#getstatusbyid) | **GET** /statuses/{statusId} | Get a specific status by ID |
| [**getStatuses**](StatusesApi.md#getstatuses) | **GET** /statuses | List statuses |
| [**updateStatusById**](StatusesApi.md#updatestatusbyid) | **PUT** /statuses/{statusId} | Update a status by ID |



## createStatus

> Status createStatus(statusCreatePayload, project)

Create a custom status

Adds a new custom status, associating it with a project specified in the payload or query.

### Example

```ts
import {
  Configuration,
  StatusesApi,
} from '@testcollab/sdk';
import type { CreateStatusRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new StatusesApi(config);

  const body = {
    // StatusCreatePayload
    statusCreatePayload: ...,
    // number | ID of the project this status belongs to.
    project: 789,
  } satisfies CreateStatusRequest;

  try {
    const data = await api.createStatus(body);
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
| **statusCreatePayload** | [StatusCreatePayload](StatusCreatePayload.md) |  | |
| **project** | `number` | ID of the project this status belongs to. | [Defaults to `undefined`] |

### Return type

[**Status**](Status.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Custom status created successfully. |  -  |
| **400** | Bad request - Invalid input data or missing project ID |  -  |
| **401** | Unauthorized - Authentication required |  -  |
| **403** | Forbidden - User does not have permission to create statuses |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteStatusById

> deleteStatusById(statusId, project)

Delete a custom status by ID

Deletes a custom status. System statuses cannot be deleted. Project context might be required.

### Example

```ts
import {
  Configuration,
  StatusesApi,
} from '@testcollab/sdk';
import type { DeleteStatusByIdRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new StatusesApi(config);

  const body = {
    // number | ID of the custom status to delete.
    statusId: 789,
    // number | ID of the project for context (if status is project-specific and needs auth check). (optional)
    project: 789,
  } satisfies DeleteStatusByIdRequest;

  try {
    const data = await api.deleteStatusById(body);
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
| **statusId** | `number` | ID of the custom status to delete. | [Defaults to `undefined`] |
| **project** | `number` | ID of the project for context (if status is project-specific and needs auth check). | [Optional] [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Status deleted successfully. |  -  |
| **400** | Bad request - Cannot delete a system status. |  -  |
| **401** | Unauthorized - Authentication required |  -  |
| **403** | Forbidden - User does not have permission to delete this status |  -  |
| **404** | Status not found |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getStatusById

> Status getStatusById(statusId, project)

Get a specific status by ID

Retrieves details of a specific status by its ID. Project context might be required for authorization.

### Example

```ts
import {
  Configuration,
  StatusesApi,
} from '@testcollab/sdk';
import type { GetStatusByIdRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new StatusesApi(config);

  const body = {
    // number | ID of the status to retrieve.
    statusId: 789,
    // number | ID of the project for context (if status is project-specific and needs auth check). (optional)
    project: 789,
  } satisfies GetStatusByIdRequest;

  try {
    const data = await api.getStatusById(body);
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
| **statusId** | `number` | ID of the status to retrieve. | [Defaults to `undefined`] |
| **project** | `number` | ID of the project for context (if status is project-specific and needs auth check). | [Optional] [Defaults to `undefined`] |

### Return type

[**Status**](Status.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Details of the status. |  -  |
| **401** | Unauthorized - Authentication required |  -  |
| **403** | Forbidden - User does not have access |  -  |
| **404** | Status not found |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getStatuses

> Array&lt;Status&gt; getStatuses(project, isActive, limit, start, sort)

List statuses

Retrieves all statuses (system and custom), optionally filtered by project.

### Example

```ts
import {
  Configuration,
  StatusesApi,
} from '@testcollab/sdk';
import type { GetStatusesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new StatusesApi(config);

  const body = {
    // number | ID of the project to filter statuses for.
    project: 789,
    // boolean | Filter statuses by active state. (optional)
    isActive: true,
    // number (optional)
    limit: 56,
    // number (optional)
    start: 56,
    // string (optional)
    sort: sort_example,
  } satisfies GetStatusesRequest;

  try {
    const data = await api.getStatuses(body);
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
| **project** | `number` | ID of the project to filter statuses for. | [Defaults to `undefined`] |
| **isActive** | `boolean` | Filter statuses by active state. | [Optional] [Defaults to `undefined`] |
| **limit** | `number` |  | [Optional] [Defaults to `undefined`] |
| **start** | `number` |  | [Optional] [Defaults to `undefined`] |
| **sort** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Status&gt;**](Status.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of statuses. |  -  |
| **400** | Bad request - Missing or invalid project ID |  -  |
| **401** | Unauthorized - Authentication required |  -  |
| **403** | Forbidden - User does not have access |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateStatusById

> Status updateStatusById(statusUpdatePayload, statusId, project)

Update a status by ID

Updates an existing status. System statuses have restrictions. Project context might be required.

### Example

```ts
import {
  Configuration,
  StatusesApi,
} from '@testcollab/sdk';
import type { UpdateStatusByIdRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new StatusesApi(config);

  const body = {
    // StatusUpdatePayload
    statusUpdatePayload: ...,
    // number | ID of the status to update.
    statusId: 789,
    // number | ID of the project for context (if status is project-specific and needs auth check). (optional)
    project: 789,
  } satisfies UpdateStatusByIdRequest;

  try {
    const data = await api.updateStatusById(body);
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
| **statusUpdatePayload** | [StatusUpdatePayload](StatusUpdatePayload.md) |  | |
| **statusId** | `number` | ID of the status to update. | [Defaults to `undefined`] |
| **project** | `number` | ID of the project for context (if status is project-specific and needs auth check). | [Optional] [Defaults to `undefined`] |

### Return type

[**Status**](Status.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Status updated successfully. |  -  |
| **400** | Bad request - Invalid input data or attempt to modify a restricted field on a system status |  -  |
| **401** | Unauthorized - Authentication required |  -  |
| **403** | Forbidden - User does not have permission to update this status |  -  |
| **404** | Status not found |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

