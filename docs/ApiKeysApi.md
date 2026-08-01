# invoicepdfs.ApiKeysApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_api_key_api_v1_api_keys_post**](ApiKeysApi.md#create_api_key_api_v1_api_keys_post) | **POST** /api/v1/api-keys | Create Api Key
[**get_api_key_api_v1_api_keys_api_key_id_get**](ApiKeysApi.md#get_api_key_api_v1_api_keys_api_key_id_get) | **GET** /api/v1/api-keys/{api_key_id} | Get Api Key
[**list_api_keys_api_v1_api_keys_get**](ApiKeysApi.md#list_api_keys_api_v1_api_keys_get) | **GET** /api/v1/api-keys | List Api Keys
[**patch_api_key_api_v1_api_keys_api_key_id_patch**](ApiKeysApi.md#patch_api_key_api_v1_api_keys_api_key_id_patch) | **PATCH** /api/v1/api-keys/{api_key_id} | Patch Api Key
[**revoke_api_key_api_v1_api_keys_api_key_id_delete**](ApiKeysApi.md#revoke_api_key_api_v1_api_keys_api_key_id_delete) | **DELETE** /api/v1/api-keys/{api_key_id} | Revoke Api Key
[**rotate_api_key_api_v1_api_keys_api_key_id_rotate_post**](ApiKeysApi.md#rotate_api_key_api_v1_api_keys_api_key_id_rotate_post) | **POST** /api/v1/api-keys/{api_key_id}/rotate | Rotate Api Key


# **create_api_key_api_v1_api_keys_post**
> ApiKeyCreateResponse create_api_key_api_v1_api_keys_post(api_key_create_request)

Create Api Key

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_create_request import ApiKeyCreateRequest
from invoicepdfs.models.api_key_create_response import ApiKeyCreateResponse
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)
    api_key_create_request = invoicepdfs.ApiKeyCreateRequest() # ApiKeyCreateRequest | 

    try:
        # Create Api Key
        api_response = api_instance.create_api_key_api_v1_api_keys_post(api_key_create_request)
        print("The response of ApiKeysApi->create_api_key_api_v1_api_keys_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->create_api_key_api_v1_api_keys_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key_create_request** | [**ApiKeyCreateRequest**](ApiKeyCreateRequest.md)|  | 

### Return type

[**ApiKeyCreateResponse**](ApiKeyCreateResponse.md)

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

# **get_api_key_api_v1_api_keys_api_key_id_get**
> ApiKeyDetailResponse get_api_key_api_v1_api_keys_api_key_id_get(api_key_id)

Get Api Key

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_detail_response import ApiKeyDetailResponse
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)
    api_key_id = 'api_key_id_example' # str | 

    try:
        # Get Api Key
        api_response = api_instance.get_api_key_api_v1_api_keys_api_key_id_get(api_key_id)
        print("The response of ApiKeysApi->get_api_key_api_v1_api_keys_api_key_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->get_api_key_api_v1_api_keys_api_key_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key_id** | **str**|  | 

### Return type

[**ApiKeyDetailResponse**](ApiKeyDetailResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_api_keys_api_v1_api_keys_get**
> ApiKeyListResponse list_api_keys_api_v1_api_keys_get()

List Api Keys

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_list_response import ApiKeyListResponse
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)

    try:
        # List Api Keys
        api_response = api_instance.list_api_keys_api_v1_api_keys_get()
        print("The response of ApiKeysApi->list_api_keys_api_v1_api_keys_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->list_api_keys_api_v1_api_keys_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiKeyListResponse**](ApiKeyListResponse.md)

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

# **patch_api_key_api_v1_api_keys_api_key_id_patch**
> ApiKeyDetailResponse patch_api_key_api_v1_api_keys_api_key_id_patch(api_key_id, api_key_patch_request)

Patch Api Key

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_detail_response import ApiKeyDetailResponse
from invoicepdfs.models.api_key_patch_request import ApiKeyPatchRequest
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)
    api_key_id = 'api_key_id_example' # str | 
    api_key_patch_request = invoicepdfs.ApiKeyPatchRequest() # ApiKeyPatchRequest | 

    try:
        # Patch Api Key
        api_response = api_instance.patch_api_key_api_v1_api_keys_api_key_id_patch(api_key_id, api_key_patch_request)
        print("The response of ApiKeysApi->patch_api_key_api_v1_api_keys_api_key_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->patch_api_key_api_v1_api_keys_api_key_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key_id** | **str**|  | 
 **api_key_patch_request** | [**ApiKeyPatchRequest**](ApiKeyPatchRequest.md)|  | 

### Return type

[**ApiKeyDetailResponse**](ApiKeyDetailResponse.md)

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

# **revoke_api_key_api_v1_api_keys_api_key_id_delete**
> ApiKeyRevokeResponse revoke_api_key_api_v1_api_keys_api_key_id_delete(api_key_id)

Revoke Api Key

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_revoke_response import ApiKeyRevokeResponse
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)
    api_key_id = 'api_key_id_example' # str | 

    try:
        # Revoke Api Key
        api_response = api_instance.revoke_api_key_api_v1_api_keys_api_key_id_delete(api_key_id)
        print("The response of ApiKeysApi->revoke_api_key_api_v1_api_keys_api_key_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->revoke_api_key_api_v1_api_keys_api_key_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key_id** | **str**|  | 

### Return type

[**ApiKeyRevokeResponse**](ApiKeyRevokeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **rotate_api_key_api_v1_api_keys_api_key_id_rotate_post**
> ApiKeyRotateResponse rotate_api_key_api_v1_api_keys_api_key_id_rotate_post(api_key_id)

Rotate Api Key

Revoke the existing key and create a new one with the same name.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_key_rotate_response import ApiKeyRotateResponse
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
    api_instance = invoicepdfs.ApiKeysApi(api_client)
    api_key_id = 'api_key_id_example' # str | 

    try:
        # Rotate Api Key
        api_response = api_instance.rotate_api_key_api_v1_api_keys_api_key_id_rotate_post(api_key_id)
        print("The response of ApiKeysApi->rotate_api_key_api_v1_api_keys_api_key_id_rotate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApiKeysApi->rotate_api_key_api_v1_api_keys_api_key_id_rotate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key_id** | **str**|  | 

### Return type

[**ApiKeyRotateResponse**](ApiKeyRotateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

