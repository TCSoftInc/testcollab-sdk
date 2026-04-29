# ExternalImportsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**cancelExternalImport**](ExternalImportsApi.md#cancelexternalimport) | **POST** /external-imports/{id}/cancel | Cancel an in-progress external import |
| [**createExternalImport**](ExternalImportsApi.md#createexternalimport) | **POST** /external-imports | Create and queue an external import job |
| [**getExternalImportStatus**](ExternalImportsApi.md#getexternalimportstatus) | **GET** /external-imports/{id}/status | Get external import status |
| [**listExternalImportAdapters**](ExternalImportsApi.md#listexternalimportadapters) | **GET** /external-imports/adapters | List available external import adapters |
| [**listExternalImportProjects**](ExternalImportsApi.md#listexternalimportprojects) | **GET** /external-imports/projects | List source-system projects available for import |
| [**testExternalImportConnection**](ExternalImportsApi.md#testexternalimportconnection) | **POST** /external-imports/test-connection | Validate external import credentials |
| [**validateExternalImportSourceProject**](ExternalImportsApi.md#validateexternalimportsourceproject) | **POST** /external-imports/validate-source-project | Validate Jira project key for external import |



## cancelExternalImport

> ExternalImportStatus cancelExternalImport(id)

Cancel an in-progress external import

Marks the import for cancellation. The runner checks the cancellation flag between batches and stops cleanly. Already-imported entities are not rolled back; the customer must delete partial entities manually if they want to start over. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { CancelExternalImportRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // number | External import job ID
    id: 18,
  } satisfies CancelExternalImportRequest;

  try {
    const data = await api.cancelExternalImport(body);
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
| **id** | `number` | External import job ID | [Defaults to `undefined`] |

### Return type

[**ExternalImportStatus**](ExternalImportStatus.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Cancellation accepted; current snapshot returned |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Import not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createExternalImport

> ExternalImportCreateResult createExternalImport(externalImportPayload)

Create and queue an external import job

Creates and queues an import job for the specified source-system project. Requires the externalImport_Run permission on the destination TestCollab project. Phase 1 blocks re-imports against the same source project; if a completed or in-progress import already exists, an error is returned. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { CreateExternalImportRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // ExternalImportPayload | Adapter type, destination project, source project, credentials and options (optional)
    externalImportPayload: ...,
  } satisfies CreateExternalImportRequest;

  try {
    const data = await api.createExternalImport(body);
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
| **externalImportPayload** | [ExternalImportPayload](ExternalImportPayload.md) | Adapter type, destination project, source project, credentials and options | [Optional] |

### Return type

[**ExternalImportCreateResult**](ExternalImportCreateResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Import job created and queued |  -  |
| **400** | Already imported, already running, or invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Permission denied |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getExternalImportStatus

> ExternalImportStatus getExternalImportStatus(id)

Get external import status

Returns a snapshot of the current status of an external import job, including stage, progress counts, per-type stats, throttle state and last activity. Frontend polls this every 2 seconds while the import is active and stops once status is done, failed, or cancelled. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { GetExternalImportStatusRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // number | External import job ID
    id: 18,
  } satisfies GetExternalImportStatusRequest;

  try {
    const data = await api.getExternalImportStatus(body);
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
| **id** | `number` | External import job ID | [Defaults to `undefined`] |

### Return type

[**ExternalImportStatus**](ExternalImportStatus.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import job status snapshot |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Import not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listExternalImportAdapters

> ExternalImportAdapterCollection listExternalImportAdapters()

List available external import adapters

Returns the list of available integration adapters with their credential field schemas and option schemas. Drives the dynamic auth form on the frontend so adding a new adapter does not require frontend changes. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { ListExternalImportAdaptersRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  try {
    const data = await api.listExternalImportAdapters();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ExternalImportAdapterCollection**](ExternalImportAdapterCollection.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of available adapters |  -  |
| **401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listExternalImportProjects

> ExternalImportSourceProjectCollection listExternalImportProjects(type, project)

List source-system projects available for import

Returns the list of projects available for import from the connected source system. Credentials must have been validated via the test-connection endpoint within the last 5 minutes (token cached server-side, keyed by user + import type). 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { ListExternalImportProjectsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // string | Adapter type (e.g. xray)
    type: xray,
    // number | Destination TestCollab project ID used to scope already_imported state
    project: 42,
  } satisfies ListExternalImportProjectsRequest;

  try {
    const data = await api.listExternalImportProjects(body);
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
| **type** | `string` | Adapter type (e.g. xray) | [Defaults to `undefined`] |
| **project** | `number` | Destination TestCollab project ID used to scope already_imported state | [Defaults to `undefined`] |

### Return type

[**ExternalImportSourceProjectCollection**](ExternalImportSourceProjectCollection.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of source projects |  -  |
| **400** | Connection token expired or missing |  -  |
| **401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## testExternalImportConnection

> ExternalImportTestConnectionResult testExternalImportConnection(externalImportTestConnectionPayload)

Validate external import credentials

Validates credentials against the source system without creating an import job. On success, the validated session is cached server-side (keyed by user + import_type) for 5 minutes so it can be reused by the project listing endpoint. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { TestExternalImportConnectionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // ExternalImportTestConnectionPayload | Adapter type and credentials to validate (optional)
    externalImportTestConnectionPayload: ...,
  } satisfies TestExternalImportConnectionRequest;

  try {
    const data = await api.testExternalImportConnection(body);
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
| **externalImportTestConnectionPayload** | [ExternalImportTestConnectionPayload](ExternalImportTestConnectionPayload.md) | Adapter type and credentials to validate | [Optional] |

### Return type

[**ExternalImportTestConnectionResult**](ExternalImportTestConnectionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Credentials are valid |  -  |
| **400** | Invalid credentials or unsupported adapter |  -  |
| **401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## validateExternalImportSourceProject

> ExternalImportValidateSourceProjectResult validateExternalImportSourceProject(externalImportValidateSourceProjectPayload)

Validate Jira project key for external import

Validates Jira credentials and a single Jira project key for the selected adapter, and returns metadata/counts for that one source project. This endpoint is used by the wizard flow that asks for a project key directly instead of loading all Jira projects. 

### Example

```ts
import {
  Configuration,
  ExternalImportsApi,
} from '@testcollab/sdk';
import type { ValidateExternalImportSourceProjectRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ExternalImportsApi(config);

  const body = {
    // ExternalImportValidateSourceProjectPayload | Adapter type, destination project, credentials and source project key (optional)
    externalImportValidateSourceProjectPayload: ...,
  } satisfies ValidateExternalImportSourceProjectRequest;

  try {
    const data = await api.validateExternalImportSourceProject(body);
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
| **externalImportValidateSourceProjectPayload** | [ExternalImportValidateSourceProjectPayload](ExternalImportValidateSourceProjectPayload.md) | Adapter type, destination project, credentials and source project key | [Optional] |

### Return type

[**ExternalImportValidateSourceProjectResult**](ExternalImportValidateSourceProjectResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Source project key is valid and accessible |  -  |
| **400** | Invalid credentials, project key, or unsupported adapter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Permission denied |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

