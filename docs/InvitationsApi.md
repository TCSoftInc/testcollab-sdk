# InvitationsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptInvitation**](InvitationsApi.md#acceptinvitation) | **PUT** /invitationsbycode/{inviteCode} | Accept invitation |
| [**createInvitation**](InvitationsApi.md#createinvitation) | **POST** /invitations | Create a new invitation |
| [**deleteInvitation**](InvitationsApi.md#deleteinvitation) | **DELETE** /invitations/{id} | Delete invitation |
| [**getInvitation**](InvitationsApi.md#getinvitation) | **GET** /invitations/{id} | Get invitation |
| [**getInvitationByCode**](InvitationsApi.md#getinvitationbycode) | **GET** /invitationsbycode/{inviteCode} | Get invitation |
| [**getInvitationCount**](InvitationsApi.md#getinvitationcount) | **GET** /invitations/count | Get count of invitations |
| [**getInvitations**](InvitationsApi.md#getinvitations) | **GET** /invitations | Get list of invitations |
| [**resendInvitation**](InvitationsApi.md#resendinvitation) | **POST** /invitations/resendInvitation | Resend invitation |
| [**updateInvitation**](InvitationsApi.md#updateinvitation) | **PUT** /invitations/{id} | Updates a invitation |



## acceptInvitation

> Invitation acceptInvitation(inviteCode)

Accept invitation

Accept invitation

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { AcceptInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Invitation Code
    inviteCode: 8.14,
  } satisfies AcceptInvitationRequest;

  try {
    const data = await api.acceptInvitation(body);
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
| **inviteCode** | `number` | Invitation Code | [Defaults to `undefined`] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createInvitation

> Invitation createInvitation(invitationPayload)

Create a new invitation

Invitation to add

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { CreateInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // InvitationPayload (optional)
    invitationPayload: ...,
  } satisfies CreateInvitationRequest;

  try {
    const data = await api.createInvitation(body);
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
| **invitationPayload** | [InvitationPayload](InvitationPayload.md) |  | [Optional] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteInvitation

> object deleteInvitation(id)

Delete invitation

Deletes a specific invitation

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { DeleteInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Invitation ID
    id: 8.14,
  } satisfies DeleteInvitationRequest;

  try {
    const data = await api.deleteInvitation(body);
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
| **id** | `number` | Invitation ID | [Defaults to `undefined`] |

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
| **200** | Invitation deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInvitation

> Invitation getInvitation(id)

Get invitation

Get details of specific invitation sent

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { GetInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Invitation ID
    id: 8.14,
  } satisfies GetInvitationRequest;

  try {
    const data = await api.getInvitation(body);
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
| **id** | `number` | Invitation ID | [Defaults to `undefined`] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInvitationByCode

> Invitation getInvitationByCode(inviteCode)

Get invitation

Get invitation code

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { GetInvitationByCodeRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const api = new InvitationsApi();

  const body = {
    // number | Invitation Code
    inviteCode: 8.14,
  } satisfies GetInvitationByCodeRequest;

  try {
    const data = await api.getInvitationByCode(body);
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
| **inviteCode** | `number` | Invitation Code | [Defaults to `undefined`] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInvitationCount

> Count getInvitationCount(company)

Get count of invitations

Get invitations\&#39; count

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { GetInvitationCountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Company ID
    company: 1,
  } satisfies GetInvitationCountRequest;

  try {
    const data = await api.getInvitationCount(body);
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
| **200** | Count of invitations |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInvitations

> Array&lt;Invitation&gt; getInvitations(limit, sort, start, filter)

Get list of invitations

Get list of invitations sent

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { GetInvitationsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Maximum number of records (optional)
    limit: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetInvitationsRequest;

  try {
    const data = await api.getInvitations(body);
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
| **limit** | `number` | Maximum number of records | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Invitation&gt;**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of invitations |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resendInvitation

> Invitation resendInvitation(invitationPayload)

Resend invitation

Invitation to add

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { ResendInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // InvitationPayload (optional)
    invitationPayload: ...,
  } satisfies ResendInvitationRequest;

  try {
    const data = await api.resendInvitation(body);
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
| **invitationPayload** | [InvitationPayload](InvitationPayload.md) |  | [Optional] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateInvitation

> Invitation updateInvitation(id, invitationPayload)

Updates a invitation

Invitation to update

### Example

```ts
import {
  Configuration,
  InvitationsApi,
} from '@testcollab/sdk';
import type { UpdateInvitationRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new InvitationsApi(config);

  const body = {
    // number | Invitation ID
    id: 8.14,
    // InvitationPayload (optional)
    invitationPayload: ...,
  } satisfies UpdateInvitationRequest;

  try {
    const data = await api.updateInvitation(body);
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
| **id** | `number` | Invitation ID | [Defaults to `undefined`] |
| **invitationPayload** | [InvitationPayload](InvitationPayload.md) |  | [Optional] |

### Return type

[**Invitation**](Invitation.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Invitation |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

