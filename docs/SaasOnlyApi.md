# SaasOnlyApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getCompanyOld**](SaasOnlyApi.md#getcompanyold) | **GET** /saasinstances/{id} | Get company info |
| [**updateCompanyBillingDetailsOld**](SaasOnlyApi.md#updatecompanybillingdetailsold) | **PUT** /saasinstances/{id} | Update billing details |



## getCompanyOld

> SaasInstance getCompanyOld(id)

Get company info

Get information specific to a company

### Example

```ts
import {
  Configuration,
  SaasOnlyApi,
} from '@testcollab/sdk';
import type { GetCompanyOldRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SaasOnlyApi(config);

  const body = {
    // number | SaaS Instance ID
    id: 8.14,
  } satisfies GetCompanyOldRequest;

  try {
    const data = await api.getCompanyOld(body);
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
| **id** | `number` | SaaS Instance ID | [Defaults to `undefined`] |

### Return type

[**SaasInstance**](SaasInstance.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | company /saas instance details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateCompanyBillingDetailsOld

> SaasInstance updateCompanyBillingDetailsOld(id, saasInstanceBillingPayload)

Update billing details

Updates billing details of specified company

### Example

```ts
import {
  Configuration,
  SaasOnlyApi,
} from '@testcollab/sdk';
import type { UpdateCompanyBillingDetailsOldRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new SaasOnlyApi(config);

  const body = {
    // number | SaaS Instance ID
    id: 8.14,
    // SaasInstanceBillingPayload (optional)
    saasInstanceBillingPayload: ...,
  } satisfies UpdateCompanyBillingDetailsOldRequest;

  try {
    const data = await api.updateCompanyBillingDetailsOld(body);
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
| **id** | `number` | SaaS Instance ID | [Defaults to `undefined`] |
| **saasInstanceBillingPayload** | [SaasInstanceBillingPayload](SaasInstanceBillingPayload.md) |  | [Optional] |

### Return type

[**SaasInstance**](SaasInstance.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | company /saas instance details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

