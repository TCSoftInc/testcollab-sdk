# IssuesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**updateIssueAttachments**](IssuesApi.md#updateissueattachments) | **PUT** /issues/{id}/updateAttachments | Update issue attachments |



## updateIssueAttachments

> Issue updateIssueAttachments(id, updateAttachmentPayload)

Update issue attachments

Issue to update

### Example

```ts
import {
  Configuration,
  IssuesApi,
} from 'testcollab-sdk';
import type { UpdateIssueAttachmentsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new IssuesApi(config);

  const body = {
    // number | Issue ID
    id: 8.14,
    // UpdateAttachmentPayload (optional)
    updateAttachmentPayload: ...,
  } satisfies UpdateIssueAttachmentsRequest;

  try {
    const data = await api.updateIssueAttachments(body);
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
| **id** | `number` | Issue ID | [Defaults to `undefined`] |
| **updateAttachmentPayload** | [UpdateAttachmentPayload](UpdateAttachmentPayload.md) |  | [Optional] |

### Return type

[**Issue**](Issue.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Issue |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

