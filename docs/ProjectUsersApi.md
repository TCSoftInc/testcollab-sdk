# ProjectUsersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProjectUser**](ProjectUsersApi.md#createprojectuser) | **POST** /projectusers | Create a new project user |
| [**deleteProjectUser**](ProjectUsersApi.md#deleteprojectuser) | **DELETE** /projectusers/{id} | Delete project member |
| [**getProjectUser**](ProjectUsersApi.md#getprojectuser) | **GET** /projectusers/{id} | Get project member |
| [**getProjectUserCount**](ProjectUsersApi.md#getprojectusercount) | **GET** /projectusers/count | Get project members\&#39; count |
| [**getProjectUserRemovalImpact**](ProjectUsersApi.md#getprojectuserremovalimpact) | **GET** /projectusers/{id}/removal-impact | Get assignment impact of removing a project member |
| [**getProjectUsers**](ProjectUsersApi.md#getprojectusers) | **GET** /projectusers | Get project users\&#39; list |
| [**removeProjectUser**](ProjectUsersApi.md#removeprojectuser) | **POST** /projectusers/{id}/remove | Remove a project member and resolve their assignments |
| [**updateProjectUser**](ProjectUsersApi.md#updateprojectuser) | **PUT** /projectusers/{id} | Updates a project user |



## createProjectUser

> ProjectUser createProjectUser(projectUserPayload)

Create a new project user

Project Member to add

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { CreateProjectUserRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // ProjectUserPayload (optional)
    projectUserPayload: ...,
  } satisfies CreateProjectUserRequest;

  try {
    const data = await api.createProjectUser(body);
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
| **projectUserPayload** | [ProjectUserPayload](ProjectUserPayload.md) |  | [Optional] |

### Return type

[**ProjectUser**](ProjectUser.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Project user |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteProjectUser

> object deleteProjectUser(id)

Delete project member

Deletes a specific project member. Only valid when the member holds no actionable assignments - use GET /projectusers/{id}/removal-impact to check, and POST /projectusers/{id}/remove to remove a member who does.

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { DeleteProjectUserRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project Member ID
    id: 8.14,
  } satisfies DeleteProjectUserRequest;

  try {
    const data = await api.deleteProjectUser(body);
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
| **id** | `number` | Project Member ID | [Defaults to `undefined`] |

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
| **200** | Project Member deleted |  -  |
| **403** | Forbidden |  -  |
| **409** | ASSIGNMENT_RESOLUTION_REQUIRED - the member holds actionable assignments that must be unassigned or reassigned first |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectUser

> ProjectUser getProjectUser(id)

Get project member

Get details of a specific project member

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { GetProjectUserRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project user ID
    id: 8.14,
  } satisfies GetProjectUserRequest;

  try {
    const data = await api.getProjectUser(body);
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
| **id** | `number` | Project user ID | [Defaults to `undefined`] |

### Return type

[**ProjectUser**](ProjectUser.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected project user |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectUserCount

> Count getProjectUserCount(project)

Get project members\&#39; count

Get project members\&#39; count

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { GetProjectUserCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
  } satisfies GetProjectUserCountRequest;

  try {
    const data = await api.getProjectUserCount(body);
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
| **200** | Count of project members |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectUserRemovalImpact

> ProjectUserRemovalImpact getProjectUserRemovalImpact(id)

Get assignment impact of removing a project member

Counts the actionable assignments held by a project member so the removal flow can decide whether the member can simply be removed or whether the assignments have to be resolved first. When total is 0 the member can be removed with DELETE /projectusers/{id}.

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { GetProjectUserRemovalImpactRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project Member ID
    id: 8.14,
  } satisfies GetProjectUserRemovalImpactRequest;

  try {
    const data = await api.getProjectUserRemovalImpact(body);
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
| **id** | `number` | Project Member ID | [Defaults to `undefined`] |

### Return type

[**ProjectUserRemovalImpact**](ProjectUserRemovalImpact.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Removal impact |  -  |
| **403** | Forbidden |  -  |
| **404** | Project member not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectUsers

> Array&lt;ProjectUser&gt; getProjectUsers(project, limit, start, sort, filter)

Get project users\&#39; list

Get details of members in a project

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { GetProjectUsersRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project ID
    project: 56,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetProjectUsersRequest;

  try {
    const data = await api.getProjectUsers(body);
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
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProjectUser&gt;**](ProjectUser.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of project users |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## removeProjectUser

> ProjectUserRemoveResult removeProjectUser(id, project, projectUserRemovePayload)

Remove a project member and resolve their assignments

Removes a project member whose actionable assignments have to be resolved first. The durable queue record is created before the membership is deleted, so a queue failure leaves the member in place. The membership is removed immediately once the job is queued; the assignments are transferred by a background job and the initiating user is notified with the result counts. Completed executions and historical records are never rewritten.

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { RemoveProjectUserRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project Member ID
    id: 8.14,
    // number | Project ID - used to scope the manageProjectMembers permission check
    project: 8.14,
    // ProjectUserRemovePayload (optional)
    projectUserRemovePayload: ...,
  } satisfies RemoveProjectUserRequest;

  try {
    const data = await api.removeProjectUser(body);
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
| **id** | `number` | Project Member ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID - used to scope the manageProjectMembers permission check | [Defaults to `undefined`] |
| **projectUserRemovePayload** | [ProjectUserRemovePayload](ProjectUserRemovePayload.md) |  | [Optional] |

### Return type

[**ProjectUserRemoveResult**](ProjectUserRemoveResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Project member removed and assignment transfer queued |  -  |
| **400** | Invalid resolution or replacement user |  -  |
| **403** | Forbidden |  -  |
| **404** | Project member not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateProjectUser

> ProjectUser updateProjectUser(id, projectUserPayload)

Updates a project user

Project Member to update

### Example

```ts
import {
  Configuration,
  ProjectUsersApi,
} from '@testcollab/sdk';
import type { UpdateProjectUserRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectUsersApi(config);

  const body = {
    // number | Project Member ID
    id: 8.14,
    // ProjectUserPayload (optional)
    projectUserPayload: ...,
  } satisfies UpdateProjectUserRequest;

  try {
    const data = await api.updateProjectUser(body);
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
| **id** | `number` | Project Member ID | [Defaults to `undefined`] |
| **projectUserPayload** | [ProjectUserPayload](ProjectUserPayload.md) |  | [Optional] |

### Return type

[**ProjectUser**](ProjectUser.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Project Member |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

