# NotificationsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**clearAll**](NotificationsApi.md#clearall) | **POST** /notifications/clearAll | Clear all notifications |
| [**deleteNotification**](NotificationsApi.md#deletenotification) | **DELETE** /notifications/{id} | Deletes given notification |
| [**getAllNotifications**](NotificationsApi.md#getallnotifications) | **GET** /notifications | Gets all notifications available in system |
| [**getMyNotifications**](NotificationsApi.md#getmynotifications) | **GET** /notifications/myNotifications | Get user\&#39;s notifications |
| [**getNotificationsCount**](NotificationsApi.md#getnotificationscount) | **GET** /notifications/count | Get count of notifications |
| [**markAsRead**](NotificationsApi.md#markasread) | **POST** /notifications/markAsRead | Mark notifications as read |
| [**markOneRead**](NotificationsApi.md#markoneread) | **POST** /notifications/markOneRead | Mark notifications as read |
| [**updateNotificationsStatus**](NotificationsApi.md#updatenotificationsstatus) | **POST** /notifications/updateStatus | Enables/Disabled given notifications for current user |



## clearAll

> object clearAll(clearAllNotificationPayload)

Clear all notifications

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { ClearAllRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // ClearAllNotificationPayload (optional)
    clearAllNotificationPayload: ...,
  } satisfies ClearAllRequest;

  try {
    const data = await api.clearAll(body);
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
| **clearAllNotificationPayload** | [ClearAllNotificationPayload](ClearAllNotificationPayload.md) |  | [Optional] |

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
| **200** | User notifications |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteNotification

> object deleteNotification(id, company)

Deletes given notification

Deletes given notification

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { DeleteNotificationRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // number | Notification ID
    id: 8.14,
    // number | Company ID
    company: 1,
  } satisfies DeleteNotificationRequest;

  try {
    const data = await api.deleteNotification(body);
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
| **id** | `number` | Notification ID | [Defaults to `undefined`] |
| **company** | `number` | Company ID | [Defaults to `undefined`] |

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
| **200** | Notification deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAllNotifications

> NotificationGroups getAllNotifications(company)

Gets all notifications available in system

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { GetAllNotificationsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // number | Company ID
    company: 1,
  } satisfies GetAllNotificationsRequest;

  try {
    const data = await api.getAllNotifications(body);
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

[**NotificationGroups**](NotificationGroups.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Available notifications in system |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMyNotifications

> Array&lt;Notification&gt; getMyNotifications(company, limit, sort, start, filter)

Get user\&#39;s notifications

Get users notifications

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { GetMyNotificationsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // string | company id
    company: company_example,
    // number | Maximum number of records (optional)
    limit: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetMyNotificationsRequest;

  try {
    const data = await api.getMyNotifications(body);
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
| **company** | `string` | company id | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Notification&gt;**](Notification.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User notifications |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getNotificationsCount

> Count getNotificationsCount(company, filter)

Get count of notifications

Get notifications\&#39; count

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { GetNotificationsCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // number | Company ID
    company: 1,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetNotificationsCountRequest;

  try {
    const data = await api.getNotificationsCount(body);
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
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

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
| **200** | Count of notifications |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## markAsRead

> object markAsRead(markAllNotificationPayload)

Mark notifications as read

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { MarkAsReadRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // MarkAllNotificationPayload (optional)
    markAllNotificationPayload: ...,
  } satisfies MarkAsReadRequest;

  try {
    const data = await api.markAsRead(body);
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
| **markAllNotificationPayload** | [MarkAllNotificationPayload](MarkAllNotificationPayload.md) |  | [Optional] |

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
| **200** | User notifications |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## markOneRead

> object markOneRead(markNotificationPayload)

Mark notifications as read

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { MarkOneReadRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // MarkNotificationPayload (optional)
    markNotificationPayload: ...,
  } satisfies MarkOneReadRequest;

  try {
    const data = await api.markOneRead(body);
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
| **markNotificationPayload** | [MarkNotificationPayload](MarkNotificationPayload.md) |  | [Optional] |

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
| **200** | User notifications |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateNotificationsStatus

> object updateNotificationsStatus(notificationPayloadCollection)

Enables/Disabled given notifications for current user

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from 'testcollab-sdk';
import type { UpdateNotificationsStatusRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationsApi(config);

  const body = {
    // NotificationPayloadCollection (optional)
    notificationPayloadCollection: ...,
  } satisfies UpdateNotificationsStatusRequest;

  try {
    const data = await api.updateNotificationsStatus(body);
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
| **notificationPayloadCollection** | [NotificationPayloadCollection](NotificationPayloadCollection.md) |  | [Optional] |

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
| **200** | Action result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

