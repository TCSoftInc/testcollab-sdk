# ReportsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getActivities**](ReportsApi.md#getactivities) | **GET** /activities | Fetch Recent Activities |
| [**getDefectTimelineReport**](ReportsApi.md#getdefecttimelinereport) | **POST** /defects/report | Get defect timeline |
| [**getDefectsTimeline**](ReportsApi.md#getdefectstimeline) | **GET** /project/tcm_reporting/tcm_reports/get_data/defectTimeline | Defects Reported |
| [**getProjectMetrics**](ReportsApi.md#getprojectmetrics) | **GET** /projects/projectMetrics | Test Metrics |
| [**getReportData**](ReportsApi.md#getreportdata) | **POST** /reports | Get timeline or any other report data |
| [**getTCFailureDistribution**](ReportsApi.md#gettcfailuredistribution) | **GET** /project/tcm_reporting/tcm_reports/get_data/testFailureDistribution | Test Cases Failure Distribution |
| [**getTestCaseLastRunStatus**](ReportsApi.md#gettestcaselastrunstatus) | **GET** /project/tcm_reporting/tcm_reports/get_data/testCaseLastStatuses | Test Cases Last Run Status |
| [**getTestCasePassedPercent**](ReportsApi.md#gettestcasepassedpercent) | **GET** /project/tcm_reporting/tcm_reports/get_data/testCasePassedPercentBySuite | Test Cases Passed % by Suite |
| [**getTestCasesProneToErrors**](ReportsApi.md#gettestcasespronetoerrors) | **GET** /project/tcm_reporting/tcm_reports/get_data/testCaseProneToErrors | Cases Prone to Errors |
| [**getTestPlanBurnDownData**](ReportsApi.md#gettestplanburndowndata) | **GET** /reports/testPlanBurnDownData | Test Plan burn down chart data |
| [**getTestPlanBurnDownDataOld**](ReportsApi.md#gettestplanburndowndataold) | **GET** /project/tcm_reporting/tcm_reports/get_data/testPlanBurnDownData | Test Plan burn down chart data |
| [**getTimeSpentPerCase**](ReportsApi.md#gettimespentpercase) | **GET** /project/tcm_reporting/tcm_reports/get_data/timeSpentPerCase | Time Spent on Each Case |



## getActivities

> Array&lt;Activity&gt; getActivities(company, user, project, entity, entityId, limit, start, sort, filter)

Fetch Recent Activities

Fetches the recent activities for a Project/Test Plan/User

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetActivitiesRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // string | Company ID
    company: 1,
    // number | User ID (optional)
    user: 56,
    // number | Project ID (optional)
    project: 56,
    // string | Possible Values - testcase / testplan / suite (optional)
    entity: testplan,
    // number | Entity ID - testplan / testcase / suite (optional)
    entityId: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetActivitiesRequest;

  try {
    const data = await api.getActivities(body);
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
| **company** | `string` | Company ID | [Defaults to `undefined`] |
| **user** | `number` | User ID | [Optional] [Defaults to `undefined`] |
| **project** | `number` | Project ID | [Optional] [Defaults to `undefined`] |
| **entity** | `string` | Possible Values - testcase / testplan / suite | [Optional] [Defaults to `undefined`] |
| **entityId** | `number` | Entity ID - testplan / testcase / suite | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Activity&gt;**](Activity.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Activities log |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDefectTimelineReport

> ReportResult getDefectTimelineReport(reportPayload)

Get defect timeline

Get defects timeline for report purpose

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetDefectTimelineReportRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // ReportPayload (optional)
    reportPayload: ...,
  } satisfies GetDefectTimelineReportRequest;

  try {
    const data = await api.getDefectTimelineReport(body);
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
| **reportPayload** | [ReportPayload](ReportPayload.md) |  | [Optional] |

### Return type

[**ReportResult**](ReportResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created Defect |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDefectsTimeline

> DefectsTimeline getDefectsTimeline(project, startDate, endDate)

Defects Reported

Defects timeline data , helps in plotting Defects Opened graph

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetDefectsTimelineRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetDefectsTimelineRequest;

  try {
    const data = await api.getDefectsTimeline(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**DefectsTimeline**](DefectsTimeline.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Defects timeline |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectMetrics

> ProjectMetrics getProjectMetrics(project, startDate, endDate)

Test Metrics

Fetches the project specific metrics

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetProjectMetricsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetProjectMetricsRequest;

  try {
    const data = await api.getProjectMetrics(body);
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
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**ProjectMetrics**](ProjectMetrics.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Project metrics |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReportData

> ReportResult getReportData(reportPayload)

Get timeline or any other report data

Get report data

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetReportDataRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // ReportPayload (optional)
    reportPayload: ...,
  } satisfies GetReportDataRequest;

  try {
    const data = await api.getReportData(body);
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
| **reportPayload** | [ReportPayload](ReportPayload.md) |  | [Optional] |

### Return type

[**ReportResult**](ReportResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Get report data |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTCFailureDistribution

> TestCaseFailureDistribution getTCFailureDistribution(project, startDate, endDate)

Test Cases Failure Distribution

Fetches the data on test case failure distribution based on the threshold selected

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTCFailureDistributionRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetTCFailureDistributionRequest;

  try {
    const data = await api.getTCFailureDistribution(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**TestCaseFailureDistribution**](TestCaseFailureDistribution.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Object having arrays of frequency and lebels (for percentage) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCaseLastRunStatus

> TestCaseLastRunStatus getTestCaseLastRunStatus(project, startDate, endDate)

Test Cases Last Run Status

Fetches summary of last run status for test cases within project

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTestCaseLastRunStatusRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetTestCaseLastRunStatusRequest;

  try {
    const data = await api.getTestCaseLastRunStatus(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**TestCaseLastRunStatus**](TestCaseLastRunStatus.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test cases last run status summary |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCasePassedPercent

> Array&lt;TestCasePassedBySuite&gt; getTestCasePassedPercent(project, startDate, endDate)

Test Cases Passed % by Suite

Fetches test cases passed percetage by suites to form the heatmap

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTestCasePassedPercentRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetTestCasePassedPercentRequest;

  try {
    const data = await api.getTestCasePassedPercent(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TestCasePassedBySuite&gt;**](TestCasePassedBySuite.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Object having arrays of frequency and lebels (for percentage) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestCasesProneToErrors

> TestCasesProneToError getTestCasesProneToErrors(project, failThreshold, startDate, endDate, limit, start, sort, filter)

Cases Prone to Errors

Fetches the data for the top 5 (max) test cases that are prone to errors based on failure threshold selected

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTestCasesProneToErrorsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // number | Used when filter on threshold is applied (optional)
    failThreshold: 50,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetTestCasesProneToErrorsRequest;

  try {
    const data = await api.getTestCasesProneToErrors(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **failThreshold** | `number` | Used when filter on threshold is applied | [Optional] [Defaults to `undefined`] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**TestCasesProneToError**](TestCasesProneToError.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Array of objects having details of top 5 (max) test cases that failed |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanBurnDownData

> ReportResult getTestPlanBurnDownData(project, testPlan)

Test Plan burn down chart data

Fetches test plan burn down chart data

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTestPlanBurnDownDataRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // number | Test Plan Id
    testPlan: 1,
  } satisfies GetTestPlanBurnDownDataRequest;

  try {
    const data = await api.getTestPlanBurnDownData(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **testPlan** | `number` | Test Plan Id | [Defaults to `undefined`] |

### Return type

[**ReportResult**](ReportResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test plan burn down chart data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTestPlanBurnDownDataOld

> TestPlanBurnDownData getTestPlanBurnDownDataOld(project, testPlan)

Test Plan burn down chart data

Fetches test plan burn down chart data

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTestPlanBurnDownDataOldRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // number | Test Plan Id
    testPlan: 1,
  } satisfies GetTestPlanBurnDownDataOldRequest;

  try {
    const data = await api.getTestPlanBurnDownDataOld(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **testPlan** | `number` | Test Plan Id | [Defaults to `undefined`] |

### Return type

[**TestPlanBurnDownData**](TestPlanBurnDownData.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test plan burn down chart data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTimeSpentPerCase

> TimeSpentPerCase getTimeSpentPerCase(project, timeSeries, startDate, endDate)

Time Spent on Each Case

Time spent on executing each test case

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@testcollab/sdk';
import type { GetTimeSpentPerCaseRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportsApi(config);

  const body = {
    // number | Project Id
    project: 1,
    // 'sum' | 'average' | 'min' | 'max' | When filter on \"time series to plot\" is applied (optional)
    timeSeries: timeSeries_example,
    // Date | Used when filter is applied (optional)
    startDate: 2019-05-01,
    // Date | Used when filter is applied (optional)
    endDate: 2019-05-10,
  } satisfies GetTimeSpentPerCaseRequest;

  try {
    const data = await api.getTimeSpentPerCase(body);
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
| **project** | `number` | Project Id | [Defaults to `undefined`] |
| **timeSeries** | `sum`, `average`, `min`, `max` | When filter on \&quot;time series to plot\&quot; is applied | [Optional] [Defaults to `undefined`] [Enum: sum, average, min, max] |
| **startDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |
| **endDate** | `Date` | Used when filter is applied | [Optional] [Defaults to `undefined`] |

### Return type

[**TimeSpentPerCase**](TimeSpentPerCase.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Objects having arrays of cases, execution counts and time spent |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

