# invoicepdfs.BatchesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_batch_api_v1_batches_batch_id_cancel_post**](BatchesApi.md#cancel_batch_api_v1_batches_batch_id_cancel_post) | **POST** /api/v1/batches/{batch_id}/cancel | Cancel Batch
[**create_batch_api_v1_batches_post**](BatchesApi.md#create_batch_api_v1_batches_post) | **POST** /api/v1/batches | Create Batch
[**download_batch_api_v1_batches_batch_id_download_get**](BatchesApi.md#download_batch_api_v1_batches_batch_id_download_get) | **GET** /api/v1/batches/{batch_id}/download | Download Batch
[**get_batch_api_v1_batches_batch_id_get**](BatchesApi.md#get_batch_api_v1_batches_batch_id_get) | **GET** /api/v1/batches/{batch_id} | Get Batch
[**list_batch_items_api_v1_batches_batch_id_items_get**](BatchesApi.md#list_batch_items_api_v1_batches_batch_id_items_get) | **GET** /api/v1/batches/{batch_id}/items | List Batch Items
[**list_batches_api_v1_batches_get**](BatchesApi.md#list_batches_api_v1_batches_get) | **GET** /api/v1/batches | List Batches


# **cancel_batch_api_v1_batches_batch_id_cancel_post**
> BatchResponse cancel_batch_api_v1_batches_batch_id_cancel_post(batch_id)

Cancel Batch

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.batch_response import BatchResponse
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
    api_instance = invoicepdfs.BatchesApi(api_client)
    batch_id = 'batch_id_example' # str | 

    try:
        # Cancel Batch
        api_response = api_instance.cancel_batch_api_v1_batches_batch_id_cancel_post(batch_id)
        print("The response of BatchesApi->cancel_batch_api_v1_batches_batch_id_cancel_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->cancel_batch_api_v1_batches_batch_id_cancel_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batch_id** | **str**|  | 

### Return type

[**BatchResponse**](BatchResponse.md)

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

# **create_batch_api_v1_batches_post**
> BatchResponse create_batch_api_v1_batches_post(batch_create_request)

Create Batch

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.batch_create_request import BatchCreateRequest
from invoicepdfs.models.batch_response import BatchResponse
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
    api_instance = invoicepdfs.BatchesApi(api_client)
    batch_create_request = invoicepdfs.BatchCreateRequest() # BatchCreateRequest | 

    try:
        # Create Batch
        api_response = api_instance.create_batch_api_v1_batches_post(batch_create_request)
        print("The response of BatchesApi->create_batch_api_v1_batches_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->create_batch_api_v1_batches_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batch_create_request** | [**BatchCreateRequest**](BatchCreateRequest.md)|  | 

### Return type

[**BatchResponse**](BatchResponse.md)

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

# **download_batch_api_v1_batches_batch_id_download_get**
> object download_batch_api_v1_batches_batch_id_download_get(batch_id)

Download Batch

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
    api_instance = invoicepdfs.BatchesApi(api_client)
    batch_id = 'batch_id_example' # str | 

    try:
        # Download Batch
        api_response = api_instance.download_batch_api_v1_batches_batch_id_download_get(batch_id)
        print("The response of BatchesApi->download_batch_api_v1_batches_batch_id_download_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->download_batch_api_v1_batches_batch_id_download_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batch_id** | **str**|  | 

### Return type

**object**

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

# **get_batch_api_v1_batches_batch_id_get**
> BatchResponse get_batch_api_v1_batches_batch_id_get(batch_id)

Get Batch

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.batch_response import BatchResponse
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
    api_instance = invoicepdfs.BatchesApi(api_client)
    batch_id = 'batch_id_example' # str | 

    try:
        # Get Batch
        api_response = api_instance.get_batch_api_v1_batches_batch_id_get(batch_id)
        print("The response of BatchesApi->get_batch_api_v1_batches_batch_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->get_batch_api_v1_batches_batch_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batch_id** | **str**|  | 

### Return type

[**BatchResponse**](BatchResponse.md)

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

# **list_batch_items_api_v1_batches_batch_id_items_get**
> BatchItemsListResponse list_batch_items_api_v1_batches_batch_id_items_get(batch_id, limit=limit, cursor=cursor)

List Batch Items

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.batch_items_list_response import BatchItemsListResponse
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
    api_instance = invoicepdfs.BatchesApi(api_client)
    batch_id = 'batch_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Batch Items
        api_response = api_instance.list_batch_items_api_v1_batches_batch_id_items_get(batch_id, limit=limit, cursor=cursor)
        print("The response of BatchesApi->list_batch_items_api_v1_batches_batch_id_items_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->list_batch_items_api_v1_batches_batch_id_items_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batch_id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**BatchItemsListResponse**](BatchItemsListResponse.md)

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

# **list_batches_api_v1_batches_get**
> BatchesListResponse list_batches_api_v1_batches_get(limit=limit, cursor=cursor)

List Batches

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.batches_list_response import BatchesListResponse
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
    api_instance = invoicepdfs.BatchesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Batches
        api_response = api_instance.list_batches_api_v1_batches_get(limit=limit, cursor=cursor)
        print("The response of BatchesApi->list_batches_api_v1_batches_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BatchesApi->list_batches_api_v1_batches_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**BatchesListResponse**](BatchesListResponse.md)

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

