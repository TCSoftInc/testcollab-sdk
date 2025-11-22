# TestPlansAssignmentApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**assignAll**](TestPlansAssignmentApi.md#assignall) | **POST** /testplans/assignAll | Assign all test cases of test plan to user |
| [**assignTestPlan**](TestPlansAssignmentApi.md#assigntestplan) | **POST** /testplans/assign | Assign test plan to users |



## assignAll

> object assignAll(testPlanAssignmentAllPayload)

Assign all test cases of test plan to user

### Example

```ts
import {
  Configuration,
  TestPlansAssignmentApi,
} from 'testcollab-sdk';
import type { AssignAllRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansAssignmentApi(config);

  const body = {
    // TestPlanAssignmentAllPayload | Assignment criteria (optional)
    testPlanAssignmentAllPayload: ...,
  } satisfies AssignAllRequest;

  try {
    const data = await api.assignAll(body);
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
| **testPlanAssignmentAllPayload** | [TestPlanAssignmentAllPayload](TestPlanAssignmentAllPayload.md) | Assignment criteria | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Assignment result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## assignTestPlan

> object assignTestPlan(testplan, project, testPlanAssignmentPayload)

Assign test plan to users

### Example

```ts
import {
  Configuration,
  TestPlansAssignmentApi,
} from 'testcollab-sdk';
import type { AssignTestPlanRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestPlansAssignmentApi(config);

  const body = {
    // number | Test Plan ID
    testplan: 1,
    // number | Project ID
    project: 1,
    // TestPlanAssignmentPayload | Assignment criteria (optional)
    testPlanAssignmentPayload: ...,
  } satisfies AssignTestPlanRequest;

  try {
    const data = await api.assignTestPlan(body);
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
| **testplan** | `number` | Test Plan ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **testPlanAssignmentPayload** | [TestPlanAssignmentPayload](TestPlanAssignmentPayload.md) | Assignment criteria | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Assignment result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

