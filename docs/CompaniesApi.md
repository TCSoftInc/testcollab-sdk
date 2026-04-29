# CompaniesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteAccount**](CompaniesApi.md#deleteaccount) | **POST** /companies/deleteAccount | Delete company account and all related data |



## deleteAccount

> DeleteAccountResult deleteAccount(deleteAccountPayload)

Delete company account and all related data

Initiates deletion of the company account and all associated data. Only the company owner (super admin) can perform this action. Deletion is processed as a background task. All data is archived to a JSON file on S3 (retained for 30 days) before deletion. 

### Example

```ts
import {
  Configuration,
  CompaniesApi,
} from '@testcollab/sdk';
import type { DeleteAccountRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CompaniesApi(config);

  const body = {
    // DeleteAccountPayload
    deleteAccountPayload: ...,
  } satisfies DeleteAccountRequest;

  try {
    const data = await api.deleteAccount(body);
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
| **deleteAccountPayload** | [DeleteAccountPayload](DeleteAccountPayload.md) |  | |

### Return type

[**DeleteAccountResult**](DeleteAccountResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deletion queued successfully |  -  |
| **400** | Bad request (company name mismatch or invalid input) |  -  |
| **403** | Forbidden (not company owner) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

