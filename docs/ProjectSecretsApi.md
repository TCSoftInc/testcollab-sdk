# ProjectSecretsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProjectSecret**](ProjectSecretsApi.md#createprojectsecret) | **POST** /projectsecrets | Create a new project secret |
| [**deleteProjectSecret**](ProjectSecretsApi.md#deleteprojectsecret) | **DELETE** /projectsecrets/{id} | Delete a project secret |
| [**getProjectSecret**](ProjectSecretsApi.md#getprojectsecret) | **GET** /projectsecrets/{id} | Get a project secret |
| [**getProjectSecrets**](ProjectSecretsApi.md#getprojectsecrets) | **GET** /projectsecrets | Get list of project secrets |
| [**getProjectSecretsCount**](ProjectSecretsApi.md#getprojectsecretscount) | **GET** /projectsecrets/count | Get project secrets count |
| [**revealProjectSecret**](ProjectSecretsApi.md#revealprojectsecret) | **GET** /projectsecrets/{id}/reveal | Reveal a project secret value |
| [**updateProjectSecret**](ProjectSecretsApi.md#updateprojectsecret) | **PUT** /projectsecrets/{id} | Update a project secret |



## createProjectSecret

> ProjectSecret createProjectSecret(projectSecretPayload)

Create a new project secret

Secret to add (value will be encrypted at rest)

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { CreateProjectSecretRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // ProjectSecretPayload (optional)
    projectSecretPayload: ...,
  } satisfies CreateProjectSecretRequest;

  try {
    const data = await api.createProjectSecret(body);
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
| **projectSecretPayload** | [ProjectSecretPayload](ProjectSecretPayload.md) |  | [Optional] |

### Return type

[**ProjectSecret**](ProjectSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created project secret (without value) |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteProjectSecret

> object deleteProjectSecret(id)

Delete a project secret

Deletes a specific project secret

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { DeleteProjectSecretRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project Secret ID
    id: 8.14,
  } satisfies DeleteProjectSecretRequest;

  try {
    const data = await api.deleteProjectSecret(body);
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
| **id** | `number` | Project Secret ID | [Defaults to `undefined`] |

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
| **200** | Project secret deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectSecret

> ProjectSecret getProjectSecret(id)

Get a project secret

Get a project secret by ID (without value)

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { GetProjectSecretRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project Secret ID
    id: 8.14,
  } satisfies GetProjectSecretRequest;

  try {
    const data = await api.getProjectSecret(body);
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
| **id** | `number` | Project Secret ID | [Defaults to `undefined`] |

### Return type

[**ProjectSecret**](ProjectSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected project secret |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectSecrets

> Array&lt;ProjectSecret&gt; getProjectSecrets(project, limit, start, sort)

Get list of project secrets

Get project-scoped secrets (values are never returned in list view)

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { GetProjectSecretsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
  } satisfies GetProjectSecretsRequest;

  try {
    const data = await api.getProjectSecrets(body);
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

### Return type

[**Array&lt;ProjectSecret&gt;**](ProjectSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of project secrets (without values) |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectSecretsCount

> Count getProjectSecretsCount(project)

Get project secrets count

Get count of secrets for a project

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { GetProjectSecretsCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project ID
    project: 1,
  } satisfies GetProjectSecretsCountRequest;

  try {
    const data = await api.getProjectSecretsCount(body);
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
| **200** | Count of project secrets |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## revealProjectSecret

> ProjectSecretRevealResult revealProjectSecret(id, project)

Reveal a project secret value

Decrypt and return the secret value. Requires secretViewValue permission.

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { RevealProjectSecretRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project Secret ID
    id: 8.14,
    // number | Project ID the secret belongs to
    project: 8.14,
  } satisfies RevealProjectSecretRequest;

  try {
    const data = await api.revealProjectSecret(body);
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
| **id** | `number` | Project Secret ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID the secret belongs to | [Defaults to `undefined`] |

### Return type

[**ProjectSecretRevealResult**](ProjectSecretRevealResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Decrypted secret value |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateProjectSecret

> ProjectSecret updateProjectSecret(id, projectSecretPayload)

Update a project secret

Secret to update

### Example

```ts
import {
  Configuration,
  ProjectSecretsApi,
} from '@testcollab/sdk';
import type { UpdateProjectSecretRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectSecretsApi(config);

  const body = {
    // number | Project Secret ID
    id: 8.14,
    // ProjectSecretPayload (optional)
    projectSecretPayload: ...,
  } satisfies UpdateProjectSecretRequest;

  try {
    const data = await api.updateProjectSecret(body);
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
| **id** | `number` | Project Secret ID | [Defaults to `undefined`] |
| **projectSecretPayload** | [ProjectSecretPayload](ProjectSecretPayload.md) |  | [Optional] |

### Return type

[**ProjectSecret**](ProjectSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated project secret (without value) |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

