# DashboardWidgetsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDashboardWidget**](DashboardWidgetsApi.md#createdashboardwidget) | **POST** /dashboardwidgets | Pin a report template to the dashboard |
| [**deleteDashboardWidget**](DashboardWidgetsApi.md#deletedashboardwidget) | **DELETE** /dashboardwidgets/{id} | Unpin a dashboard widget |
| [**getDashboardWidgets**](DashboardWidgetsApi.md#getdashboardwidgets) | **GET** /dashboardwidgets | Get list of pinned dashboard widgets |
| [**setDashboardWidgetSortOrder**](DashboardWidgetsApi.md#setdashboardwidgetsortorder) | **POST** /dashboardwidgets/setSortOrder | Set display order of dashboard widgets |



## createDashboardWidget

> DashboardWidget createDashboardWidget(dashboardWidgetPayload)

Pin a report template to the dashboard

Pin a saved report template as a dashboard widget

### Example

```ts
import {
  Configuration,
  DashboardWidgetsApi,
} from '@testcollab/sdk';
import type { CreateDashboardWidgetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DashboardWidgetsApi(config);

  const body = {
    // DashboardWidgetPayload (optional)
    dashboardWidgetPayload: ...,
  } satisfies CreateDashboardWidgetRequest;

  try {
    const data = await api.createDashboardWidget(body);
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
| **dashboardWidgetPayload** | [DashboardWidgetPayload](DashboardWidgetPayload.md) |  | [Optional] |

### Return type

[**DashboardWidget**](DashboardWidget.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Created dashboard widget |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteDashboardWidget

> object deleteDashboardWidget(id)

Unpin a dashboard widget

Remove a pinned report template from the dashboard

### Example

```ts
import {
  Configuration,
  DashboardWidgetsApi,
} from '@testcollab/sdk';
import type { DeleteDashboardWidgetRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DashboardWidgetsApi(config);

  const body = {
    // number | Dashboard Widget ID
    id: 8.14,
  } satisfies DeleteDashboardWidgetRequest;

  try {
    const data = await api.deleteDashboardWidget(body);
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
| **id** | `number` | Dashboard Widget ID | [Defaults to `undefined`] |

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
| **200** | Dashboard widget removed |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDashboardWidgets

> Array&lt;DashboardWidget&gt; getDashboardWidgets(project, sort)

Get list of pinned dashboard widgets

Get list of report templates pinned to a project\&#39;s dashboard

### Example

```ts
import {
  Configuration,
  DashboardWidgetsApi,
} from '@testcollab/sdk';
import type { GetDashboardWidgetsRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DashboardWidgetsApi(config);

  const body = {
    // number | Project ID
    project: 1,
    // string | Sort according to a specific field (optional)
    sort: sort_example,
  } satisfies GetDashboardWidgetsRequest;

  try {
    const data = await api.getDashboardWidgets(body);
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
| **sort** | `string` | Sort according to a specific field | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;DashboardWidget&gt;**](DashboardWidget.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of dashboard widgets |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setDashboardWidgetSortOrder

> object setDashboardWidgetSortOrder(dashboardWidgetSortOrderPayload)

Set display order of dashboard widgets

Reorder pinned dashboard widgets

### Example

```ts
import {
  Configuration,
  DashboardWidgetsApi,
} from '@testcollab/sdk';
import type { SetDashboardWidgetSortOrderRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DashboardWidgetsApi(config);

  const body = {
    // DashboardWidgetSortOrderPayload (optional)
    dashboardWidgetSortOrderPayload: ...,
  } satisfies SetDashboardWidgetSortOrderRequest;

  try {
    const data = await api.setDashboardWidgetSortOrder(body);
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
| **dashboardWidgetSortOrderPayload** | [DashboardWidgetSortOrderPayload](DashboardWidgetSortOrderPayload.md) |  | [Optional] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Sort order updated |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

