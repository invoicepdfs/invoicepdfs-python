# invoicepdfs.AuthApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**exchange_auth_token**](AuthApi.md#exchange_auth_token) | **POST** /api/v1/auth/token | Exchange Auth Token
[**get_current_user**](AuthApi.md#get_current_user) | **GET** /api/v1/auth/me | Get Current User
[**logout**](AuthApi.md#logout) | **POST** /api/v1/auth/logout | Logout
[**refresh_access_token**](AuthApi.md#refresh_access_token) | **POST** /api/v1/auth/refresh | Refresh Access Token
[**register**](AuthApi.md#register) | **POST** /api/v1/auth/register | Register
[**request_password_reset**](AuthApi.md#request_password_reset) | **POST** /api/v1/auth/forgot-password | Request Password Reset
[**reset_password**](AuthApi.md#reset_password) | **POST** /api/v1/auth/reset-password | Reset Password
[**update_current_user**](AuthApi.md#update_current_user) | **PATCH** /api/v1/auth/me | Update Current User


# **exchange_auth_token**
> AuthTokenResponse exchange_auth_token(auth_token_request)

Exchange Auth Token

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
        # Exchange Auth Token
        api_response = api_instance.exchange_auth_token(auth_token_request)
        print("The response of AuthApi->exchange_auth_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->exchange_auth_token: %s\n" % e)
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

# **get_current_user**
> AuthMeResponse get_current_user()

Get Current User

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
        # Get Current User
        api_response = api_instance.get_current_user()
        print("The response of AuthApi->get_current_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->get_current_user: %s\n" % e)
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

# **logout**
> AuthMessageResponse logout()

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
        api_response = api_instance.logout()
        print("The response of AuthApi->logout:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->logout: %s\n" % e)
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

# **refresh_access_token**
> AuthRefreshResponse refresh_access_token(auth_refresh_request)

Refresh Access Token

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
        # Refresh Access Token
        api_response = api_instance.refresh_access_token(auth_refresh_request)
        print("The response of AuthApi->refresh_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->refresh_access_token: %s\n" % e)
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

# **register**
> AuthRegisterResponse register(auth_register_request)

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
        api_response = api_instance.register(auth_register_request)
        print("The response of AuthApi->register:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->register: %s\n" % e)
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

# **request_password_reset**
> AuthMessageResponse request_password_reset(auth_forgot_password_request)

Request Password Reset

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
        # Request Password Reset
        api_response = api_instance.request_password_reset(auth_forgot_password_request)
        print("The response of AuthApi->request_password_reset:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->request_password_reset: %s\n" % e)
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

# **reset_password**
> AuthMessageResponse reset_password(auth_reset_password_request)

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
        api_response = api_instance.reset_password(auth_reset_password_request)
        print("The response of AuthApi->reset_password:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->reset_password: %s\n" % e)
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

# **update_current_user**
> AuthMeResponse update_current_user(auth_me_patch_request)

Update Current User

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
        # Update Current User
        api_response = api_instance.update_current_user(auth_me_patch_request)
        print("The response of AuthApi->update_current_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->update_current_user: %s\n" % e)
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

