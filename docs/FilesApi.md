# invoicepdfs.FilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_file_api_v1_files_file_id_delete**](FilesApi.md#delete_file_api_v1_files_file_id_delete) | **DELETE** /api/v1/files/{file_id} | Delete File
[**get_file_api_v1_files_file_id_get**](FilesApi.md#get_file_api_v1_files_file_id_get) | **GET** /api/v1/files/{file_id} | Get File
[**upload_file_api_v1_files_post**](FilesApi.md#upload_file_api_v1_files_post) | **POST** /api/v1/files | Upload File


# **delete_file_api_v1_files_file_id_delete**
> SimpleBoolResponse delete_file_api_v1_files_file_id_delete(file_id)

Delete File

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
    api_instance = invoicepdfs.FilesApi(api_client)
    file_id = 'file_id_example' # str | 

    try:
        # Delete File
        api_response = api_instance.delete_file_api_v1_files_file_id_delete(file_id)
        print("The response of FilesApi->delete_file_api_v1_files_file_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->delete_file_api_v1_files_file_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file_id** | **str**|  | 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_file_api_v1_files_file_id_get**
> FileResponse get_file_api_v1_files_file_id_get(file_id)

Get File

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.file_response import FileResponse
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
    api_instance = invoicepdfs.FilesApi(api_client)
    file_id = 'file_id_example' # str | 

    try:
        # Get File
        api_response = api_instance.get_file_api_v1_files_file_id_get(file_id)
        print("The response of FilesApi->get_file_api_v1_files_file_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->get_file_api_v1_files_file_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file_id** | **str**|  | 

### Return type

[**FileResponse**](FileResponse.md)

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

# **upload_file_api_v1_files_post**
> FileResponse upload_file_api_v1_files_post(file, idempotency_key=idempotency_key)

Upload File

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.file_response import FileResponse
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
    api_instance = invoicepdfs.FilesApi(api_client)
    file = None # bytearray | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Upload File
        api_response = api_instance.upload_file_api_v1_files_post(file, idempotency_key=idempotency_key)
        print("The response of FilesApi->upload_file_api_v1_files_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->upload_file_api_v1_files_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**FileResponse**](FileResponse.md)

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

