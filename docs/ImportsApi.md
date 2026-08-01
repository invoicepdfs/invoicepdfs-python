# invoicepdfs.ImportsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_import_api_v1_imports_import_id_cancel_post**](ImportsApi.md#cancel_import_api_v1_imports_import_id_cancel_post) | **POST** /api/v1/imports/{import_id}/cancel | Cancel Import
[**confirm_import_api_v1_imports_import_id_confirm_post**](ImportsApi.md#confirm_import_api_v1_imports_import_id_confirm_post) | **POST** /api/v1/imports/{import_id}/confirm | Confirm Import
[**create_import_api_v1_imports_post**](ImportsApi.md#create_import_api_v1_imports_post) | **POST** /api/v1/imports | Create Import
[**get_import_api_v1_imports_import_id_get**](ImportsApi.md#get_import_api_v1_imports_import_id_get) | **GET** /api/v1/imports/{import_id} | Get Import


# **cancel_import_api_v1_imports_import_id_cancel_post**
> ImportResponse cancel_import_api_v1_imports_import_id_cancel_post(import_id)

Cancel Import

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.import_response import ImportResponse
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
    api_instance = invoicepdfs.ImportsApi(api_client)
    import_id = 'import_id_example' # str | 

    try:
        # Cancel Import
        api_response = api_instance.cancel_import_api_v1_imports_import_id_cancel_post(import_id)
        print("The response of ImportsApi->cancel_import_api_v1_imports_import_id_cancel_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ImportsApi->cancel_import_api_v1_imports_import_id_cancel_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **import_id** | **str**|  | 

### Return type

[**ImportResponse**](ImportResponse.md)

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

# **confirm_import_api_v1_imports_import_id_confirm_post**
> ImportResponse confirm_import_api_v1_imports_import_id_confirm_post(import_id)

Confirm Import

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.import_response import ImportResponse
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
    api_instance = invoicepdfs.ImportsApi(api_client)
    import_id = 'import_id_example' # str | 

    try:
        # Confirm Import
        api_response = api_instance.confirm_import_api_v1_imports_import_id_confirm_post(import_id)
        print("The response of ImportsApi->confirm_import_api_v1_imports_import_id_confirm_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ImportsApi->confirm_import_api_v1_imports_import_id_confirm_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **import_id** | **str**|  | 

### Return type

[**ImportResponse**](ImportResponse.md)

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

# **create_import_api_v1_imports_post**
> ImportResponse create_import_api_v1_imports_post(import_create_request)

Create Import

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.import_create_request import ImportCreateRequest
from invoicepdfs.models.import_response import ImportResponse
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
    api_instance = invoicepdfs.ImportsApi(api_client)
    import_create_request = invoicepdfs.ImportCreateRequest() # ImportCreateRequest | 

    try:
        # Create Import
        api_response = api_instance.create_import_api_v1_imports_post(import_create_request)
        print("The response of ImportsApi->create_import_api_v1_imports_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ImportsApi->create_import_api_v1_imports_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **import_create_request** | [**ImportCreateRequest**](ImportCreateRequest.md)|  | 

### Return type

[**ImportResponse**](ImportResponse.md)

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

# **get_import_api_v1_imports_import_id_get**
> ImportResponse get_import_api_v1_imports_import_id_get(import_id)

Get Import

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.import_response import ImportResponse
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
    api_instance = invoicepdfs.ImportsApi(api_client)
    import_id = 'import_id_example' # str | 

    try:
        # Get Import
        api_response = api_instance.get_import_api_v1_imports_import_id_get(import_id)
        print("The response of ImportsApi->get_import_api_v1_imports_import_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ImportsApi->get_import_api_v1_imports_import_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **import_id** | **str**|  | 

### Return type

[**ImportResponse**](ImportResponse.md)

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

