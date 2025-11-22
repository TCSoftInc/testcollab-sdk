# ProjectsettingsApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteProjectSetting**](ProjectsettingsApi.md#deleteprojectsetting) | **DELETE** /projectsettings | Deletes settings for given project |
| [**getProjectSettings**](ProjectsettingsApi.md#getprojectsettings) | **GET** /projectsettings | Project specific settings |
| [**setProjectSettings**](ProjectsettingsApi.md#setprojectsettings) | **POST** /projectsettings | Save settings |



## deleteProjectSetting

> object deleteProjectSetting(project, filter)

Deletes settings for given project

Deletes settings for given project

### Example

```ts
import {
  Configuration,
  ProjectsettingsApi,
} from 'testcollab-sdk';
import type { DeleteProjectSettingRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectsettingsApi(config);

  const body = {
    // number | project ID
    project: 8.14,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies DeleteProjectSettingRequest;

  try {
    const data = await api.deleteProjectSetting(body);
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
| **project** | `number` | project ID | [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

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
| **200** | Setting deleted |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProjectSettings

> Array&lt;Projectsetting&gt; getProjectSettings(project, settingType, limit, filter)

Project specific settings

Get details of project specific settings

### Example

```ts
import {
  Configuration,
  ProjectsettingsApi,
} from 'testcollab-sdk';
import type { GetProjectSettingsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectsettingsApi(config);

  const body = {
    // number | Project ID
    project: 8.14,
    // string | setting type like general, email (optional)
    settingType: settingType_example,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetProjectSettingsRequest;

  try {
    const data = await api.getProjectSettings(body);
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
| **settingType** | `string` | setting type like general, email | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Projectsetting&gt;**](Projectsetting.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of settings for requested type (project wise) |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setProjectSettings

> GenericActionResult setProjectSettings(projectsettingPayload)

Save settings

settings to save

### Example

```ts
import {
  Configuration,
  ProjectsettingsApi,
} from 'testcollab-sdk';
import type { SetProjectSettingsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ProjectsettingsApi(config);

  const body = {
    // ProjectsettingPayload (optional)
    projectsettingPayload: ...,
  } satisfies SetProjectSettingsRequest;

  try {
    const data = await api.setProjectSettings(body);
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
| **projectsettingPayload** | [ProjectsettingPayload](ProjectsettingPayload.md) |  | [Optional] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Settings saved |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

