# invoicepdfs.BrandingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_logo_api_v1_branding_logo_delete**](BrandingApi.md#delete_logo_api_v1_branding_logo_delete) | **DELETE** /api/v1/branding/logo | Delete Logo
[**get_branding_api_v1_branding_get**](BrandingApi.md#get_branding_api_v1_branding_get) | **GET** /api/v1/branding | Get Branding
[**update_branding_api_v1_branding_put**](BrandingApi.md#update_branding_api_v1_branding_put) | **PUT** /api/v1/branding | Update Branding
[**upload_logo_api_v1_branding_logo_post**](BrandingApi.md#upload_logo_api_v1_branding_logo_post) | **POST** /api/v1/branding/logo | Upload Logo


# **delete_logo_api_v1_branding_logo_delete**
> SimpleBoolResponse delete_logo_api_v1_branding_logo_delete()

Delete Logo

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.simple_bool_response import SimpleBoolResponse
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
    api_instance = invoicepdfs.BrandingApi(api_client)

    try:
        # Delete Logo
        api_response = api_instance.delete_logo_api_v1_branding_logo_delete()
        print("The response of BrandingApi->delete_logo_api_v1_branding_logo_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingApi->delete_logo_api_v1_branding_logo_delete: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SimpleBoolResponse**](SimpleBoolResponse.md)

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

# **get_branding_api_v1_branding_get**
> BrandingResponse get_branding_api_v1_branding_get()

Get Branding

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_response import BrandingResponse
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
    api_instance = invoicepdfs.BrandingApi(api_client)

    try:
        # Get Branding
        api_response = api_instance.get_branding_api_v1_branding_get()
        print("The response of BrandingApi->get_branding_api_v1_branding_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingApi->get_branding_api_v1_branding_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**BrandingResponse**](BrandingResponse.md)

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

# **update_branding_api_v1_branding_put**
> BrandingResponse update_branding_api_v1_branding_put(branding_update_request)

Update Branding

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_response import BrandingResponse
from invoicepdfs.models.branding_update_request import BrandingUpdateRequest
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
    api_instance = invoicepdfs.BrandingApi(api_client)
    branding_update_request = invoicepdfs.BrandingUpdateRequest() # BrandingUpdateRequest | 

    try:
        # Update Branding
        api_response = api_instance.update_branding_api_v1_branding_put(branding_update_request)
        print("The response of BrandingApi->update_branding_api_v1_branding_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingApi->update_branding_api_v1_branding_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **branding_update_request** | [**BrandingUpdateRequest**](BrandingUpdateRequest.md)|  | 

### Return type

[**BrandingResponse**](BrandingResponse.md)

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

# **upload_logo_api_v1_branding_logo_post**
> BrandingResponse upload_logo_api_v1_branding_logo_post(file)

Upload Logo

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_response import BrandingResponse
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
    api_instance = invoicepdfs.BrandingApi(api_client)
    file = None # bytearray | 

    try:
        # Upload Logo
        api_response = api_instance.upload_logo_api_v1_branding_logo_post(file)
        print("The response of BrandingApi->upload_logo_api_v1_branding_logo_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingApi->upload_logo_api_v1_branding_logo_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**|  | 

### Return type

[**BrandingResponse**](BrandingResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

