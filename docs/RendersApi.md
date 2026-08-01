# invoicepdfs.RendersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_render_api_v1_renders_render_id_download_get**](RendersApi.md#download_render_api_v1_renders_render_id_download_get) | **GET** /api/v1/renders/{render_id}/download | Download Render
[**get_render_api_v1_renders_render_id_get**](RendersApi.md#get_render_api_v1_renders_render_id_get) | **GET** /api/v1/renders/{render_id} | Get Render


# **download_render_api_v1_renders_render_id_download_get**
> bytearray download_render_api_v1_renders_render_id_download_get(render_id)

Download Render

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
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
    api_instance = invoicepdfs.RendersApi(api_client)
    render_id = 'render_id_example' # str | 

    try:
        # Download Render
        api_response = api_instance.download_render_api_v1_renders_render_id_download_get(render_id)
        print("The response of RendersApi->download_render_api_v1_renders_render_id_download_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RendersApi->download_render_api_v1_renders_render_id_download_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **render_id** | **str**|  | 

### Return type

**bytearray**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | PDF file |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_render_api_v1_renders_render_id_get**
> Dict[str, object] get_render_api_v1_renders_render_id_get(render_id)

Get Render

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
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
    api_instance = invoicepdfs.RendersApi(api_client)
    render_id = 'render_id_example' # str | 

    try:
        # Get Render
        api_response = api_instance.get_render_api_v1_renders_render_id_get(render_id)
        print("The response of RendersApi->get_render_api_v1_renders_render_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RendersApi->get_render_api_v1_renders_render_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **render_id** | **str**|  | 

### Return type

**Dict[str, object]**

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

