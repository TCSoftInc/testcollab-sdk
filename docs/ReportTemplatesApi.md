# ReportTemplatesApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getReportTemplateResults**](ReportTemplatesApi.md#getreporttemplateresults) | **GET** /reporttemplates/{id}/results | Get results of a saved report |



## getReportTemplateResults

> ReportTemplateResults getReportTemplateResults(id, dateFrom, dateTo)

Get results of a saved report

Runs a report that was already built in TestCollab and returns its aggregated rows. The report is identified by its id and its definition is resolved on the server, so nothing about how the report is built has to be sent with the request - which is what makes this endpoint suitable for a scheduled extract into a BI tool or a monitoring check.  Each row carries one key per dimension (the grouped value) and one key per metric (the computed number); &#x60;dimensions&#x60; and &#x60;metrics&#x60; describe those keys in order, so a client can map the rows to columns without knowing the report.  A report shared with the project (\&quot;Public\&quot;) can be run by any member of the project; a \&quot;Private\&quot; report only by the person who created it.

### Example

```ts
import {
  Configuration,
  ReportTemplatesApi,
} from '@testcollab/sdk';
import type { GetReportTemplateResultsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ReportTemplatesApi(config);

  const body = {
    // number | Report ID
    id: 12,
    // string | Start of the window (YYYY-MM-DD) to run the report over, replacing the date range saved with the report. Must be sent together with date_to, and the two cannot be more than 365 days apart. Omit both to use the report\'s own range. (optional)
    dateFrom: 2026-08-01,
    // string | End of the window (YYYY-MM-DD), sent together with date_from (optional)
    dateTo: 2026-08-31,
  } satisfies GetReportTemplateResultsRequest;

  try {
    const data = await api.getReportTemplateResults(body);
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
| **id** | `number` | Report ID | [Defaults to `undefined`] |
| **dateFrom** | `string` | Start of the window (YYYY-MM-DD) to run the report over, replacing the date range saved with the report. Must be sent together with date_to, and the two cannot be more than 365 days apart. Omit both to use the report\&#39;s own range. | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` | End of the window (YYYY-MM-DD), sent together with date_from | [Optional] [Defaults to `undefined`] |

### Return type

[**ReportTemplateResults**](ReportTemplateResults.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Report results |  -  |
| **400** | Invalid date_from/date_to, or the report matches more records than a single run may aggregate |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Report not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

