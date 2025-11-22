# UsersApi

All URIs are relative to *https://api.testcollab.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**confirmUser**](UsersApi.md#confirmuser) | **GET** /auth/email-confirmation | Confirm user signup |
| [**createUser**](UsersApi.md#createuser) | **POST** /auth/local/register | Create a new user |
| [**deleteUser**](UsersApi.md#deleteuser) | **DELETE** /users/{userID} | Delete user |
| [**downgradeAdmin**](UsersApi.md#downgradeadmin) | **POST** /users/downgrade/{id} | Downgrade administrator to user |
| [**editUser**](UsersApi.md#edituser) | **PUT** /users/{userID} | Edit user |
| [**forgotPassword**](UsersApi.md#forgotpassword) | **POST** /auth/forgot-password | Sends the reset password email to user |
| [**getMyIssueManagers**](UsersApi.md#getmyissuemanagers) | **GET** /users/getMyIssueManagers | Get issue managers user can link to |
| [**getMyUser**](UsersApi.md#getmyuser) | **GET** /users/me | Get user |
| [**getUser**](UsersApi.md#getuser) | **GET** /users/{userID} | Get user |
| [**getUserProfile**](UsersApi.md#getuserprofile) | **GET** /users/profile | Get user profile |
| [**getUsers**](UsersApi.md#getusers) | **GET** /users | Get users |
| [**getUsersCount**](UsersApi.md#getuserscount) | **GET** /users/count | Get users\&#39; count |
| [**login**](UsersApi.md#login) | **POST** /auth/local | Login |
| [**logout**](UsersApi.md#logout) | **GET** /users/logout | Logout user |
| [**resendVerfication**](UsersApi.md#resendverfication) | **POST** /users/resendVerification | Resend verification email |
| [**resetAllPasswords**](UsersApi.md#resetallpasswords) | **POST** /users/resetAllPasswords | Reset all passwords |
| [**resetPassword**](UsersApi.md#resetpassword) | **POST** /auth/reset-password | Reset Password |
| [**sendVerfication**](UsersApi.md#sendverfication) | **POST** /users/sendVerification | Send verification email |
| [**setSuperAdmin**](UsersApi.md#setsuperadmin) | **POST** /users/changeSuperAdmin | Upgrades a user as super administrator |
| [**setupProfile**](UsersApi.md#setupprofile) | **PUT** /setupProfile | Setup profile when user is invited |
| [**upgradeUser**](UsersApi.md#upgradeuser) | **POST** /users/upgrade/{id} | Upgrades a user to an administrator |
| [**verfiyEmail**](UsersApi.md#verfiyemail) | **POST** /users/verifyEmail | Verify email |



## confirmUser

> confirmUser(confirmation)

Confirm user signup

Confirm user\&#39;s email with the code

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { ConfirmUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // string | Confirmation code from email
    confirmation: 456lkjdflgj5343,
  } satisfies ConfirmUserRequest;

  try {
    const data = await api.confirmUser(body);
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
| **confirmation** | `string` | Confirmation code from email | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **302** | Email is confirmed |  -  |
| **500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createUser

> RegisteredUser createUser(userCreatePayload)

Create a new user

This will create a new user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { CreateUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // UserCreatePayload | user creds (optional)
    userCreatePayload: ...,
  } satisfies CreateUserRequest;

  try {
    const data = await api.createUser(body);
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
| **userCreatePayload** | [UserCreatePayload](UserCreatePayload.md) | user creds | [Optional] |

### Return type

[**RegisteredUser**](RegisteredUser.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logged in user with JWT |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteUser

> object deleteUser(userID, company)

Delete user

Deletes a user and his/her associations with all project of company

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { DeleteUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | User ID
    userID: 1,
    // number | Company ID
    company: 1,
  } satisfies DeleteUserRequest;

  try {
    const data = await api.deleteUser(body);
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
| **userID** | `number` | User ID | [Defaults to `undefined`] |
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
| **200** | result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## downgradeAdmin

> object downgradeAdmin(id, company)

Downgrade administrator to user

Downgrades an administrator to user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { DowngradeAdminRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | User ID
    id: 1,
    // number | Company ID
    company: 1,
  } satisfies DowngradeAdminRequest;

  try {
    const data = await api.downgradeAdmin(body);
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
| **id** | `number` | User ID | [Defaults to `undefined`] |
| **company** | `number` | Company ID | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## editUser

> User editUser(userID, userEditPayload)

Edit user

If user is admin, he can edit any user\&#39;s profile, otherwise he can only edit his own profile 

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { EditUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | User ID
    userID: 1,
    // UserEditPayload | Edited user; Except id all other fields are optional (optional)
    userEditPayload: ...,
  } satisfies EditUserRequest;

  try {
    const data = await api.editUser(body);
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
| **userID** | `number` | User ID | [Defaults to `undefined`] |
| **userEditPayload** | [UserEditPayload](UserEditPayload.md) | Edited user; Except id all other fields are optional | [Optional] |

### Return type

[**User**](User.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## forgotPassword

> object forgotPassword(forgotPasswordPayload)

Sends the reset password email to user

Sends the instructions to reset password via email to id provided with request

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { ForgotPasswordRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // ForgotPasswordPayload (optional)
    forgotPasswordPayload: ...,
  } satisfies ForgotPasswordRequest;

  try {
    const data = await api.forgotPassword(body);
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
| **forgotPasswordPayload** | [ForgotPasswordPayload](ForgotPasswordPayload.md) |  | [Optional] |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Email found in the database |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Email not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMyIssueManagers

> Array&lt;ProjectsettingMini&gt; getMyIssueManagers()

Get issue managers user can link to

Get issue managers user can link to

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetMyIssueManagersRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  try {
    const data = await api.getMyIssueManagers();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;ProjectsettingMini&gt;**](ProjectsettingMini.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | user details |  -  |
| **400** | bad input parameter |  -  |
| **404** | user not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMyUser

> UserMy getMyUser()

Get user

Get currently logged in user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetMyUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  try {
    const data = await api.getMyUser();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserMy**](UserMy.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUser

> User getUser(userID, company)

Get user

Get details of a specific user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | User ID
    userID: 1,
    // number | Company ID
    company: 1,
  } satisfies GetUserRequest;

  try {
    const data = await api.getUser(body);
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
| **userID** | `number` | User ID | [Defaults to `undefined`] |
| **company** | `number` | Company ID | [Defaults to `undefined`] |

### Return type

[**User**](User.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | user details |  -  |
| **400** | bad input parameter |  -  |
| **404** | user not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUserProfile

> User getUserProfile(username)

Get user profile

Get profile of a specific user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetUserProfileRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // string | Username
    username: shritig,
  } satisfies GetUserProfileRequest;

  try {
    const data = await api.getUserProfile(body);
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
| **username** | `string` | Username | [Defaults to `undefined`] |

### Return type

[**User**](User.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | user profile details |  -  |
| **400** | bad input parameter |  -  |
| **404** | user not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUsers

> Array&lt;User&gt; getUsers(company, limit, start, sort, filter)

Get users

Get list of all users in a company

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetUsersRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | Company ID
    company: 1,
    // number | Limit the size of the returned results (optional)
    limit: 56,
    // number | Skip a specific number of entries (for pagination) (optional)
    start: 56,
    // string | Sort according to a specific field. (optional)
    sort: sort_example,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetUsersRequest;

  try {
    const data = await api.getUsers(body);
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
| **limit** | `number` | Limit the size of the returned results | [Optional] [Defaults to `undefined`] |
| **start** | `number` | Skip a specific number of entries (for pagination) | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Sort according to a specific field. | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;User&gt;**](User.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Users array |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUsersCount

> Count getUsersCount(company, filter)

Get users\&#39; count

Get users\&#39; count for a specific company

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { GetUsersCountRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | Company ID
    company: 8.14,
    // string | Stringified filter object  (https://strapi.io/documentation/developer-docs/latest/development/plugins/graphql.html#filters) (optional)
    filter: filter_example,
  } satisfies GetUsersCountRequest;

  try {
    const data = await api.getUsersCount(body);
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
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Count of users |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## login

> LoggedInUser login(userLoginPayload)

Login

To get JWT for logged  in user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { LoginRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // UserLoginPayload | user creds (optional)
    userLoginPayload: ...,
  } satisfies LoginRequest;

  try {
    const data = await api.login(body);
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
| **userLoginPayload** | [UserLoginPayload](UserLoginPayload.md) | user creds | [Optional] |

### Return type

[**LoggedInUser**](LoggedInUser.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logged in user with JWT |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## logout

> GenericActionResult logout()

Logout user

Logout a user

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { LogoutRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  try {
    const data = await api.logout();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | logout |  -  |
| **400** | bad input parameter |  -  |
| **404** | user not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resendVerfication

> GenericActionResult resendVerfication(sendVerificationPayload)

Resend verification email

Resend verification email

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { ResendVerficationRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // SendVerificationPayload | Email where verification to be sent (optional)
    sendVerificationPayload: ...,
  } satisfies ResendVerficationRequest;

  try {
    const data = await api.resendVerfication(body);
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
| **sendVerificationPayload** | [SendVerificationPayload](SendVerificationPayload.md) | Email where verification to be sent | [Optional] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Generic Action result |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resetAllPasswords

> GenericActionResult resetAllPasswords(resetAllPasswordPayload)

Reset all passwords

Reset all passwords due to password policy changes

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { ResetAllPasswordsRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // ResetAllPasswordPayload | Reset all passwords due to password policy changes (optional)
    resetAllPasswordPayload: ...,
  } satisfies ResetAllPasswordsRequest;

  try {
    const data = await api.resetAllPasswords(body);
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
| **resetAllPasswordPayload** | [ResetAllPasswordPayload](ResetAllPasswordPayload.md) | Reset all passwords due to password policy changes | [Optional] |

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
| **200** | Generic Action result |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resetPassword

> RegisteredUser resetPassword(resetPasswordPayload)

Reset Password

This will reset user\&#39;s password

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { ResetPasswordRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // ResetPasswordPayload | user creds (optional)
    resetPasswordPayload: ...,
  } satisfies ResetPasswordRequest;

  try {
    const data = await api.resetPassword(body);
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
| **resetPasswordPayload** | [ResetPasswordPayload](ResetPasswordPayload.md) | user creds | [Optional] |

### Return type

[**RegisteredUser**](RegisteredUser.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logged in user with JWT |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendVerfication

> GenericActionResult sendVerfication(sendVerificationPayload)

Send verification email

Send verification email 

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { SendVerficationRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // SendVerificationPayload | Email where verification to be sent (optional)
    sendVerificationPayload: ...,
  } satisfies SendVerficationRequest;

  try {
    const data = await api.sendVerfication(body);
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
| **sendVerificationPayload** | [SendVerificationPayload](SendVerificationPayload.md) | Email where verification to be sent | [Optional] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Generic Action result |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setSuperAdmin

> GenericActionResult setSuperAdmin(changeSuperAdminPayload)

Upgrades a user as super administrator

Upgrades a user as super administrator

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { SetSuperAdminRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // ChangeSuperAdminPayload (optional)
    changeSuperAdminPayload: ...,
  } satisfies SetSuperAdminRequest;

  try {
    const data = await api.setSuperAdmin(body);
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
| **changeSuperAdminPayload** | [ChangeSuperAdminPayload](ChangeSuperAdminPayload.md) |  | [Optional] |

### Return type

[**GenericActionResult**](GenericActionResult.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setupProfile

> User setupProfile(setupProfilePayload)

Setup profile when user is invited

If user is admin, he can edit any user, otherwise he can only edit his own profile 

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { SetupProfileRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // SetupProfilePayload | Edited user; Except id all other fields are optional (optional)
    setupProfilePayload: ...,
  } satisfies SetupProfileRequest;

  try {
    const data = await api.setupProfile(body);
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
| **setupProfilePayload** | [SetupProfilePayload](SetupProfilePayload.md) | Edited user; Except id all other fields are optional | [Optional] |

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Action status details |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## upgradeUser

> object upgradeUser(id, company)

Upgrades a user to an administrator

Upgrades a user to an administrator

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { UpgradeUserRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
    // To configure API key authorization: bearerAuth
    apiKey: "YOUR API KEY",
  });
  const api = new UsersApi(config);

  const body = {
    // number | User ID
    id: 1,
    // number | Company ID
    company: 1,
  } satisfies UpgradeUserRequest;

  try {
    const data = await api.upgradeUser(body);
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
| **id** | `number` | User ID | [Defaults to `undefined`] |
| **company** | `number` | Company ID | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | result |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |
| **0** | Unexpected error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## verfiyEmail

> LoggedInUser verfiyEmail(verifyEmailPayload)

Verify email

Send verification email 

### Example

```ts
import {
  Configuration,
  UsersApi,
} from 'testcollab-sdk';
import type { VerfiyEmailRequest } from 'testcollab-sdk';

async function example() {
  console.log("🚀 Testing testcollab-sdk SDK...");
  const api = new UsersApi();

  const body = {
    // VerifyEmailPayload | Confirmation code (optional)
    verifyEmailPayload: ...,
  } satisfies VerfiyEmailRequest;

  try {
    const data = await api.verfiyEmail(body);
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
| **verifyEmailPayload** | [VerifyEmailPayload](VerifyEmailPayload.md) | Confirmation code | [Optional] |

### Return type

[**LoggedInUser**](LoggedInUser.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Verified user |  -  |
| **400** | bad input parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

