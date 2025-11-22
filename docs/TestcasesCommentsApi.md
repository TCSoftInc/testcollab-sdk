# TestcasesCommentsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addTestCaseComment**](TestcasesCommentsApi.md#addtestcasecomment) | **POST** /testcasecomments | Add test case comment |
| [**deleteTestCaseComment**](TestcasesCommentsApi.md#deletetestcasecomment) | **DELETE** /testcasecomments/{id} | Delete test case comment |
| [**getTestCaseComment**](TestcasesCommentsApi.md#gettestcasecomment) | **GET** /testcasecomments/{id} | Get test case comment |
| [**getTestCaseComments**](TestcasesCommentsApi.md#gettestcasecomments) | **GET** /testcasecomments | Get test case comments |
| [**getTestCaseCommentsCount**](TestcasesCommentsApi.md#gettestcasecommentscount) | **GET** /testcasecomments/count | Get test case comments\&#39;count |
| [**updateTestCaseComment**](TestcasesCommentsApi.md#updatetestcasecomment) | **PUT** /testcasecomments/{id} | Updates a test case comment |



## addTestCaseComment

> TestCaseComment addTestCaseComment(testCaseCommentPayload)

Add test case comment

Adds a new test case comment

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { AddTestCaseCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // TestCaseCommentPayload | Comment to add (optional)
    testCaseCommentPayload: ...,
  } satisfies AddTestCaseCommentRequest;

  try {
    const data = await api.addTestCaseComment(body);
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
| **testCaseCommentPayload** | [TestCaseCommentPayload](TestCaseCommentPayload.md) | Comment to add | [Optional] |

### Return type

[**TestCaseComment**](TestCaseComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created TestCaseComment |  -  |
| **400** | bad input parameter |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTestCaseComment

> object deleteTestCaseComment(id, project)

Delete test case comment

Delete a specific comment added for a test case

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { DeleteTestCaseCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // number | Test Case Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies DeleteTestCaseCommentRequest;

  try {
    const data = await api.deleteTestCaseComment(body);
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
| **id** | `number` | Test Case Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

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
| **200** | Test Case Comment deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseComment

> TestCaseComment getTestCaseComment(id, project)

Get test case comment

Get comments added for a specific test case

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { GetTestCaseCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // number | Test Case Comment ID
    id: 8.14,
    // number | Project ID
    project: 8.14,
  } satisfies GetTestCaseCommentRequest;

  try {
    const data = await api.getTestCaseComment(body);
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
| **id** | `number` | Test Case Comment ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |

### Return type

[**TestCaseComment**](TestCaseComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Selected test case |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseComments

> Array&lt;TestCaseComment&gt; getTestCaseComments(testCase, project, limit, start, sort, filter)

Get test case comments

Get comments for a specific test case

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { GetTestCaseCommentsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // number | Test case ID
    testCase: 1,
    // number | Project ID
    project: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestCaseCommentsRequest;

  try {
    const data = await api.getTestCaseComments(body);
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
| **testCase** | `number` | Test case ID | [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestCaseComment&gt;**](TestCaseComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test case comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseCommentsCount

> Count getTestCaseCommentsCount(project, testCase)

Get test case comments\&#39;count

Get count of comments added for a specific test case

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { GetTestCaseCommentsCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // number | Test Plan ID
    testCase: 8.14,
  } satisfies GetTestCaseCommentsCountRequest;

  try {
    const data = await api.getTestCaseCommentsCount(body);
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
| **testCase** | `number` | Test Plan ID | [Defaults to `undefined`] |

### Return type

[**Count**](Count.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of test case comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTestCaseComment

> TestCaseComment updateTestCaseComment(id, testCaseCommentPayload)

Updates a test case comment

Test Case to update

### Example

```ts
import {
  Configuration,
  TestcasesCommentsApi,
} from 'testcollab-sdk';
import type { UpdateTestCaseCommentRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TestcasesCommentsApi(config);

  const body = {
    // number | Test Case Comment ID
    id: 8.14,
    // TestCaseCommentPayload (optional)
    testCaseCommentPayload: ...,
  } satisfies UpdateTestCaseCommentRequest;

  try {
    const data = await api.updateTestCaseComment(body);
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
| **id** | `number` | Test Case Comment ID | [Defaults to `undefined`] |
| **testCaseCommentPayload** | [TestCaseCommentPayload](TestCaseCommentPayload.md) |  | [Optional] |

### Return type

[**TestCaseComment**](TestCaseComment.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated Test Case comment |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

