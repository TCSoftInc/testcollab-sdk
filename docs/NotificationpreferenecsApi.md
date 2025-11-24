# NotificationpreferenecsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createNotificationPreference**](NotificationpreferenecsApi.md#createnotificationpreference) | **POST** /notificationpreferences | Create a new notification preference |
| [**getMyNotificationPreference**](NotificationpreferenecsApi.md#getmynotificationpreference) | **GET** /notificationpreferences/myPreferences | Get a notification preference |
| [**getNotificationPreference**](NotificationpreferenecsApi.md#getnotificationpreference) | **GET** /notificationpreferences/{id} | Get a notification preference |
| [**updateNotificationPreference**](NotificationpreferenecsApi.md#updatenotificationpreference) | **PUT** /notificationpreferences/{id} | Update notification preference |



## createNotificationPreference

> NotificationPreference createNotificationPreference(notificationPreferencePayload)

Create a new notification preference

Add notification preference

### Example

```ts
import {
  Configuration,
  NotificationpreferenecsApi,
} from '@testcollab/sdk';
import type { CreateNotificationPreferenceRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationpreferenecsApi(config);

  const body = {
    // NotificationPreferencePayload (optional)
    notificationPreferencePayload: ...,
  } satisfies CreateNotificationPreferenceRequest;

  try {
    const data = await api.createNotificationPreference(body);
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
| **notificationPreferencePayload** | [NotificationPreferencePayload](NotificationPreferencePayload.md) |  | [Optional] |

### Return type

[**NotificationPreference**](NotificationPreference.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Create notification preference |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMyNotificationPreference

> NotificationPreference getMyNotificationPreference(company)

Get a notification preference

### Example

```ts
import {
  Configuration,
  NotificationpreferenecsApi,
} from '@testcollab/sdk';
import type { GetMyNotificationPreferenceRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationpreferenecsApi(config);

  const body = {
    // number | Company ID
    company: 8.14,
  } satisfies GetMyNotificationPreferenceRequest;

  try {
    const data = await api.getMyNotificationPreference(body);
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

[**NotificationPreference**](NotificationPreference.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Get notification preference |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getNotificationPreference

> NotificationPreference getNotificationPreference(id)

Get a notification preference

### Example

```ts
import {
  Configuration,
  NotificationpreferenecsApi,
} from '@testcollab/sdk';
import type { GetNotificationPreferenceRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationpreferenecsApi(config);

  const body = {
    // number | Notification preference ID
    id: 8.14,
  } satisfies GetNotificationPreferenceRequest;

  try {
    const data = await api.getNotificationPreference(body);
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
| **id** | `number` | Notification preference ID | [Defaults to `undefined`] |

### Return type

[**NotificationPreference**](NotificationPreference.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Get notification preference |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateNotificationPreference

> NotificationPreference updateNotificationPreference(id, notificationPreferencePayload)

Update notification preference

### Example

```ts
import {
  Configuration,
  NotificationpreferenecsApi,
} from '@testcollab/sdk';
import type { UpdateNotificationPreferenceRequest } from '@testcollab/sdk';

async function example() {
  console.log("🚀 Testing @testcollab/sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new NotificationpreferenecsApi(config);

  const body = {
    // number | Notification preference ID
    id: 8.14,
    // NotificationPreferencePayload (optional)
    notificationPreferencePayload: ...,
  } satisfies UpdateNotificationPreferenceRequest;

  try {
    const data = await api.updateNotificationPreference(body);
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
| **id** | `number` | Notification preference ID | [Defaults to `undefined`] |
| **notificationPreferencePayload** | [NotificationPreferencePayload](NotificationPreferencePayload.md) |  | [Optional] |

### Return type

[**NotificationPreference**](NotificationPreference.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Update notification preference |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

