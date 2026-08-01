# invoicepdfs.AuthApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**forgot_password_api_v1_auth_forgot_password_post**](AuthApi.md#forgot_password_api_v1_auth_forgot_password_post) | **POST** /api/v1/auth/forgot-password | Forgot Password
[**logout_api_v1_auth_logout_post**](AuthApi.md#logout_api_v1_auth_logout_post) | **POST** /api/v1/auth/logout | Logout
[**me_api_v1_auth_me_get**](AuthApi.md#me_api_v1_auth_me_get) | **GET** /api/v1/auth/me | Me
[**patch_me_api_v1_auth_me_patch**](AuthApi.md#patch_me_api_v1_auth_me_patch) | **PATCH** /api/v1/auth/me | Patch Me
[**refresh_api_v1_auth_refresh_post**](AuthApi.md#refresh_api_v1_auth_refresh_post) | **POST** /api/v1/auth/refresh | Refresh
[**register_api_v1_auth_register_post**](AuthApi.md#register_api_v1_auth_register_post) | **POST** /api/v1/auth/register | Register
[**reset_password_api_v1_auth_reset_password_post**](AuthApi.md#reset_password_api_v1_auth_reset_password_post) | **POST** /api/v1/auth/reset-password | Reset Password
[**token_exchange_api_v1_auth_token_post**](AuthApi.md#token_exchange_api_v1_auth_token_post) | **POST** /api/v1/auth/token | Token Exchange


# **forgot_password_api_v1_auth_forgot_password_post**
> AuthMessageResponse forgot_password_api_v1_auth_forgot_password_post(auth_forgot_password_request)

Forgot Password

Send a password reset email via Firebase.

### Example


```python
import invoicepdfs
from invoicepdfs.models.auth_forgot_password_request import AuthForgotPasswordRequest
from invoicepdfs.models.auth_message_response import AuthMessageResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_forgot_password_request = invoicepdfs.AuthForgotPasswordRequest() # AuthForgotPasswordRequest | 

    try:
        # Forgot Password
        api_response = api_instance.forgot_password_api_v1_auth_forgot_password_post(auth_forgot_password_request)
        print("The response of AuthApi->forgot_password_api_v1_auth_forgot_password_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->forgot_password_api_v1_auth_forgot_password_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_forgot_password_request** | [**AuthForgotPasswordRequest**](AuthForgotPasswordRequest.md)|  | 

### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logout_api_v1_auth_logout_post**
> AuthMessageResponse logout_api_v1_auth_logout_post()

Logout

Revoke all Firebase refresh tokens for the authenticated user.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.auth_message_response import AuthMessageResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)

    try:
        # Logout
        api_response = api_instance.logout_api_v1_auth_logout_post()
        print("The response of AuthApi->logout_api_v1_auth_logout_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->logout_api_v1_auth_logout_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **me_api_v1_auth_me_get**
> AuthMeResponse me_api_v1_auth_me_get()

Me

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.auth_me_response import AuthMeResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)

    try:
        # Me
        api_response = api_instance.me_api_v1_auth_me_get()
        print("The response of AuthApi->me_api_v1_auth_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->me_api_v1_auth_me_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AuthMeResponse**](AuthMeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_me_api_v1_auth_me_patch**
> AuthMeResponse patch_me_api_v1_auth_me_patch(auth_me_patch_request)

Patch Me

Update the authenticated account's name or email.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.auth_me_patch_request import AuthMePatchRequest
from invoicepdfs.models.auth_me_response import AuthMeResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_me_patch_request = invoicepdfs.AuthMePatchRequest() # AuthMePatchRequest | 

    try:
        # Patch Me
        api_response = api_instance.patch_me_api_v1_auth_me_patch(auth_me_patch_request)
        print("The response of AuthApi->patch_me_api_v1_auth_me_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->patch_me_api_v1_auth_me_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_me_patch_request** | [**AuthMePatchRequest**](AuthMePatchRequest.md)|  | 

### Return type

[**AuthMeResponse**](AuthMeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refresh_api_v1_auth_refresh_post**
> AuthRefreshResponse refresh_api_v1_auth_refresh_post(auth_refresh_request)

Refresh

Exchange a Firebase refresh token for a new ID token.

### Example


```python
import invoicepdfs
from invoicepdfs.models.auth_refresh_request import AuthRefreshRequest
from invoicepdfs.models.auth_refresh_response import AuthRefreshResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_refresh_request = invoicepdfs.AuthRefreshRequest() # AuthRefreshRequest | 

    try:
        # Refresh
        api_response = api_instance.refresh_api_v1_auth_refresh_post(auth_refresh_request)
        print("The response of AuthApi->refresh_api_v1_auth_refresh_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->refresh_api_v1_auth_refresh_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_refresh_request** | [**AuthRefreshRequest**](AuthRefreshRequest.md)|  | 

### Return type

[**AuthRefreshResponse**](AuthRefreshResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register_api_v1_auth_register_post**
> AuthRegisterResponse register_api_v1_auth_register_post(auth_register_request)

Register

Register a new account using a Firebase ID token.  The client authenticates with Firebase (email/password, Google, etc.) and sends the resulting ID token here to create an InvoicePDFs account.

### Example


```python
import invoicepdfs
from invoicepdfs.models.auth_register_request import AuthRegisterRequest
from invoicepdfs.models.auth_register_response import AuthRegisterResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_register_request = invoicepdfs.AuthRegisterRequest() # AuthRegisterRequest | 

    try:
        # Register
        api_response = api_instance.register_api_v1_auth_register_post(auth_register_request)
        print("The response of AuthApi->register_api_v1_auth_register_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->register_api_v1_auth_register_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_register_request** | [**AuthRegisterRequest**](AuthRegisterRequest.md)|  | 

### Return type

[**AuthRegisterResponse**](AuthRegisterResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reset_password_api_v1_auth_reset_password_post**
> AuthMessageResponse reset_password_api_v1_auth_reset_password_post(auth_reset_password_request)

Reset Password

Confirm a password reset using the code from the reset email.

### Example


```python
import invoicepdfs
from invoicepdfs.models.auth_message_response import AuthMessageResponse
from invoicepdfs.models.auth_reset_password_request import AuthResetPasswordRequest
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_reset_password_request = invoicepdfs.AuthResetPasswordRequest() # AuthResetPasswordRequest | 

    try:
        # Reset Password
        api_response = api_instance.reset_password_api_v1_auth_reset_password_post(auth_reset_password_request)
        print("The response of AuthApi->reset_password_api_v1_auth_reset_password_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->reset_password_api_v1_auth_reset_password_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_reset_password_request** | [**AuthResetPasswordRequest**](AuthResetPasswordRequest.md)|  | 

### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **token_exchange_api_v1_auth_token_post**
> AuthTokenResponse token_exchange_api_v1_auth_token_post(auth_token_request)

Token Exchange

Exchange a Firebase ID token for account info.  Use this on login: the client authenticates with Firebase, sends the ID token here, and receives the InvoicePDFs account details. The Firebase token itself is used as the Bearer token for subsequent API calls.

### Example


```python
import invoicepdfs
from invoicepdfs.models.auth_token_request import AuthTokenRequest
from invoicepdfs.models.auth_token_response import AuthTokenResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.AuthApi(api_client)
    auth_token_request = invoicepdfs.AuthTokenRequest() # AuthTokenRequest | 

    try:
        # Token Exchange
        api_response = api_instance.token_exchange_api_v1_auth_token_post(auth_token_request)
        print("The response of AuthApi->token_exchange_api_v1_auth_token_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->token_exchange_api_v1_auth_token_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth_token_request** | [**AuthTokenRequest**](AuthTokenRequest.md)|  | 

### Return type

[**AuthTokenResponse**](AuthTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

