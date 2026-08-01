# invoicepdfs.DocumentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**archive_document_api_v1_documents_document_id_archive_post**](DocumentsApi.md#archive_document_api_v1_documents_document_id_archive_post) | **POST** /api/v1/documents/{document_id}/archive | Archive Document
[**calculate_document_api_v1_documents_calculate_post**](DocumentsApi.md#calculate_document_api_v1_documents_calculate_post) | **POST** /api/v1/documents/calculate | Calculate Document
[**create_document_api_v1_documents_post**](DocumentsApi.md#create_document_api_v1_documents_post) | **POST** /api/v1/documents | Create Document
[**delete_document_api_v1_documents_document_id_delete**](DocumentsApi.md#delete_document_api_v1_documents_document_id_delete) | **DELETE** /api/v1/documents/{document_id} | Delete Document
[**duplicate_document_api_v1_documents_document_id_duplicate_post**](DocumentsApi.md#duplicate_document_api_v1_documents_document_id_duplicate_post) | **POST** /api/v1/documents/{document_id}/duplicate | Duplicate Document
[**finalize_document_api_v1_documents_document_id_finalize_post**](DocumentsApi.md#finalize_document_api_v1_documents_document_id_finalize_post) | **POST** /api/v1/documents/{document_id}/finalize | Finalize Document
[**get_document_api_v1_documents_document_id_get**](DocumentsApi.md#get_document_api_v1_documents_document_id_get) | **GET** /api/v1/documents/{document_id} | Get Document
[**list_document_deliveries_api_v1_documents_document_id_deliveries_get**](DocumentsApi.md#list_document_deliveries_api_v1_documents_document_id_deliveries_get) | **GET** /api/v1/documents/{document_id}/deliveries | List Document Deliveries
[**list_documents_api_v1_documents_get**](DocumentsApi.md#list_documents_api_v1_documents_get) | **GET** /api/v1/documents | List Documents
[**mark_paid_api_v1_documents_document_id_mark_paid_post**](DocumentsApi.md#mark_paid_api_v1_documents_document_id_mark_paid_post) | **POST** /api/v1/documents/{document_id}/mark-paid | Mark Paid
[**mark_sent_api_v1_documents_document_id_mark_sent_post**](DocumentsApi.md#mark_sent_api_v1_documents_document_id_mark_sent_post) | **POST** /api/v1/documents/{document_id}/mark-sent | Mark Sent
[**mark_unpaid_api_v1_documents_document_id_mark_unpaid_post**](DocumentsApi.md#mark_unpaid_api_v1_documents_document_id_mark_unpaid_post) | **POST** /api/v1/documents/{document_id}/mark-unpaid | Mark Unpaid
[**patch_document_api_v1_documents_document_id_patch**](DocumentsApi.md#patch_document_api_v1_documents_document_id_patch) | **PATCH** /api/v1/documents/{document_id} | Patch Document
[**render_document_api_v1_documents_document_id_renders_post**](DocumentsApi.md#render_document_api_v1_documents_document_id_renders_post) | **POST** /api/v1/documents/{document_id}/renders | Render Document
[**render_document_api_v1_documents_render_post**](DocumentsApi.md#render_document_api_v1_documents_render_post) | **POST** /api/v1/documents/render | Render Document
[**restore_document_api_v1_documents_document_id_restore_post**](DocumentsApi.md#restore_document_api_v1_documents_document_id_restore_post) | **POST** /api/v1/documents/{document_id}/restore | Restore Document
[**send_document_api_v1_documents_document_id_send_post**](DocumentsApi.md#send_document_api_v1_documents_document_id_send_post) | **POST** /api/v1/documents/{document_id}/send | Send Document
[**validate_document_api_v1_documents_validate_post**](DocumentsApi.md#validate_document_api_v1_documents_validate_post) | **POST** /api/v1/documents/validate | Validate Document
[**void_document_api_v1_documents_document_id_void_post**](DocumentsApi.md#void_document_api_v1_documents_document_id_void_post) | **POST** /api/v1/documents/{document_id}/void | Void Document


# **archive_document_api_v1_documents_document_id_archive_post**
> DocumentResponse archive_document_api_v1_documents_document_id_archive_post(document_id)

Archive Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Archive Document
        api_response = api_instance.archive_document_api_v1_documents_document_id_archive_post(document_id)
        print("The response of DocumentsApi->archive_document_api_v1_documents_document_id_archive_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->archive_document_api_v1_documents_document_id_archive_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **calculate_document_api_v1_documents_calculate_post**
> DocumentCalculateResponse calculate_document_api_v1_documents_calculate_post(document_calculate_request)

Calculate Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_calculate_request import DocumentCalculateRequest
from invoicepdfs.models.document_calculate_response import DocumentCalculateResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_calculate_request = invoicepdfs.DocumentCalculateRequest() # DocumentCalculateRequest | 

    try:
        # Calculate Document
        api_response = api_instance.calculate_document_api_v1_documents_calculate_post(document_calculate_request)
        print("The response of DocumentsApi->calculate_document_api_v1_documents_calculate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->calculate_document_api_v1_documents_calculate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_calculate_request** | [**DocumentCalculateRequest**](DocumentCalculateRequest.md)|  | 

### Return type

[**DocumentCalculateResponse**](DocumentCalculateResponse.md)

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

# **create_document_api_v1_documents_post**
> DocumentResponse create_document_api_v1_documents_post(document_create_request, idempotency_key=idempotency_key)

Create Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_create_request import DocumentCreateRequest
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_create_request = invoicepdfs.DocumentCreateRequest() # DocumentCreateRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Document
        api_response = api_instance.create_document_api_v1_documents_post(document_create_request, idempotency_key=idempotency_key)
        print("The response of DocumentsApi->create_document_api_v1_documents_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->create_document_api_v1_documents_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_create_request** | [**DocumentCreateRequest**](DocumentCreateRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **delete_document_api_v1_documents_document_id_delete**
> SimpleBoolResponse delete_document_api_v1_documents_document_id_delete(document_id)

Delete Document

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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Delete Document
        api_response = api_instance.delete_document_api_v1_documents_document_id_delete(document_id)
        print("The response of DocumentsApi->delete_document_api_v1_documents_document_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->delete_document_api_v1_documents_document_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

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

# **duplicate_document_api_v1_documents_document_id_duplicate_post**
> DocumentResponse duplicate_document_api_v1_documents_document_id_duplicate_post(document_id)

Duplicate Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Duplicate Document
        api_response = api_instance.duplicate_document_api_v1_documents_document_id_duplicate_post(document_id)
        print("The response of DocumentsApi->duplicate_document_api_v1_documents_document_id_duplicate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->duplicate_document_api_v1_documents_document_id_duplicate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **finalize_document_api_v1_documents_document_id_finalize_post**
> DocumentResponse finalize_document_api_v1_documents_document_id_finalize_post(document_id)

Finalize Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Finalize Document
        api_response = api_instance.finalize_document_api_v1_documents_document_id_finalize_post(document_id)
        print("The response of DocumentsApi->finalize_document_api_v1_documents_document_id_finalize_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->finalize_document_api_v1_documents_document_id_finalize_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **get_document_api_v1_documents_document_id_get**
> DocumentResponse get_document_api_v1_documents_document_id_get(document_id)

Get Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Get Document
        api_response = api_instance.get_document_api_v1_documents_document_id_get(document_id)
        print("The response of DocumentsApi->get_document_api_v1_documents_document_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->get_document_api_v1_documents_document_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **list_document_deliveries_api_v1_documents_document_id_deliveries_get**
> DeliveriesListResponse list_document_deliveries_api_v1_documents_document_id_deliveries_get(document_id, limit=limit, cursor=cursor)

List Document Deliveries

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.deliveries_list_response import DeliveriesListResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Document Deliveries
        api_response = api_instance.list_document_deliveries_api_v1_documents_document_id_deliveries_get(document_id, limit=limit, cursor=cursor)
        print("The response of DocumentsApi->list_document_deliveries_api_v1_documents_document_id_deliveries_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->list_document_deliveries_api_v1_documents_document_id_deliveries_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**DeliveriesListResponse**](DeliveriesListResponse.md)

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

# **list_documents_api_v1_documents_get**
> DocumentsListResponse list_documents_api_v1_documents_get(limit=limit, cursor=cursor, document_type=document_type, status=status)

List Documents

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.documents_list_response import DocumentsListResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)
    document_type = 'document_type_example' # str |  (optional)
    status = 'status_example' # str |  (optional)

    try:
        # List Documents
        api_response = api_instance.list_documents_api_v1_documents_get(limit=limit, cursor=cursor, document_type=document_type, status=status)
        print("The response of DocumentsApi->list_documents_api_v1_documents_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->list_documents_api_v1_documents_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 
 **document_type** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 

### Return type

[**DocumentsListResponse**](DocumentsListResponse.md)

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

# **mark_paid_api_v1_documents_document_id_mark_paid_post**
> DocumentResponse mark_paid_api_v1_documents_document_id_mark_paid_post(document_id)

Mark Paid

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Mark Paid
        api_response = api_instance.mark_paid_api_v1_documents_document_id_mark_paid_post(document_id)
        print("The response of DocumentsApi->mark_paid_api_v1_documents_document_id_mark_paid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->mark_paid_api_v1_documents_document_id_mark_paid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **mark_sent_api_v1_documents_document_id_mark_sent_post**
> DocumentResponse mark_sent_api_v1_documents_document_id_mark_sent_post(document_id)

Mark Sent

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Mark Sent
        api_response = api_instance.mark_sent_api_v1_documents_document_id_mark_sent_post(document_id)
        print("The response of DocumentsApi->mark_sent_api_v1_documents_document_id_mark_sent_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->mark_sent_api_v1_documents_document_id_mark_sent_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **mark_unpaid_api_v1_documents_document_id_mark_unpaid_post**
> DocumentResponse mark_unpaid_api_v1_documents_document_id_mark_unpaid_post(document_id)

Mark Unpaid

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Mark Unpaid
        api_response = api_instance.mark_unpaid_api_v1_documents_document_id_mark_unpaid_post(document_id)
        print("The response of DocumentsApi->mark_unpaid_api_v1_documents_document_id_mark_unpaid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->mark_unpaid_api_v1_documents_document_id_mark_unpaid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **patch_document_api_v1_documents_document_id_patch**
> DocumentResponse patch_document_api_v1_documents_document_id_patch(document_id, document_patch_request)

Patch Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_patch_request import DocumentPatchRequest
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 
    document_patch_request = invoicepdfs.DocumentPatchRequest() # DocumentPatchRequest | 

    try:
        # Patch Document
        api_response = api_instance.patch_document_api_v1_documents_document_id_patch(document_id, document_patch_request)
        print("The response of DocumentsApi->patch_document_api_v1_documents_document_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->patch_document_api_v1_documents_document_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **document_patch_request** | [**DocumentPatchRequest**](DocumentPatchRequest.md)|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **render_document_api_v1_documents_document_id_renders_post**
> object render_document_api_v1_documents_document_id_renders_post(document_id, app_documents_schemas_document_render_request, idempotency_key=idempotency_key)

Render Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.app_documents_schemas_document_render_request import AppDocumentsSchemasDocumentRenderRequest
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 
    app_documents_schemas_document_render_request = invoicepdfs.AppDocumentsSchemasDocumentRenderRequest() # AppDocumentsSchemasDocumentRenderRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Render Document
        api_response = api_instance.render_document_api_v1_documents_document_id_renders_post(document_id, app_documents_schemas_document_render_request, idempotency_key=idempotency_key)
        print("The response of DocumentsApi->render_document_api_v1_documents_document_id_renders_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->render_document_api_v1_documents_document_id_renders_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **app_documents_schemas_document_render_request** | [**AppDocumentsSchemasDocumentRenderRequest**](AppDocumentsSchemasDocumentRenderRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

**object**

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

# **render_document_api_v1_documents_render_post**
> object render_document_api_v1_documents_render_post(app_schemas_v1_document_render_request, idempotency_key=idempotency_key)

Render Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.app_schemas_v1_document_render_request import AppSchemasV1DocumentRenderRequest
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    app_schemas_v1_document_render_request = invoicepdfs.AppSchemasV1DocumentRenderRequest() # AppSchemasV1DocumentRenderRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Render Document
        api_response = api_instance.render_document_api_v1_documents_render_post(app_schemas_v1_document_render_request, idempotency_key=idempotency_key)
        print("The response of DocumentsApi->render_document_api_v1_documents_render_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->render_document_api_v1_documents_render_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_schemas_v1_document_render_request** | [**AppSchemasV1DocumentRenderRequest**](AppSchemasV1DocumentRenderRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

**object**

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

# **restore_document_api_v1_documents_document_id_restore_post**
> DocumentResponse restore_document_api_v1_documents_document_id_restore_post(document_id)

Restore Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Restore Document
        api_response = api_instance.restore_document_api_v1_documents_document_id_restore_post(document_id)
        print("The response of DocumentsApi->restore_document_api_v1_documents_document_id_restore_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->restore_document_api_v1_documents_document_id_restore_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

# **send_document_api_v1_documents_document_id_send_post**
> DeliveryResponse send_document_api_v1_documents_document_id_send_post(document_id, delivery_send_request)

Send Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.delivery_response import DeliveryResponse
from invoicepdfs.models.delivery_send_request import DeliverySendRequest
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 
    delivery_send_request = invoicepdfs.DeliverySendRequest() # DeliverySendRequest | 

    try:
        # Send Document
        api_response = api_instance.send_document_api_v1_documents_document_id_send_post(document_id, delivery_send_request)
        print("The response of DocumentsApi->send_document_api_v1_documents_document_id_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->send_document_api_v1_documents_document_id_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **delivery_send_request** | [**DeliverySendRequest**](DeliverySendRequest.md)|  | 

### Return type

[**DeliveryResponse**](DeliveryResponse.md)

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

# **validate_document_api_v1_documents_validate_post**
> DocumentValidateResponse validate_document_api_v1_documents_validate_post(document_validate_request)

Validate Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_validate_request import DocumentValidateRequest
from invoicepdfs.models.document_validate_response import DocumentValidateResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_validate_request = invoicepdfs.DocumentValidateRequest() # DocumentValidateRequest | 

    try:
        # Validate Document
        api_response = api_instance.validate_document_api_v1_documents_validate_post(document_validate_request)
        print("The response of DocumentsApi->validate_document_api_v1_documents_validate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->validate_document_api_v1_documents_validate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_validate_request** | [**DocumentValidateRequest**](DocumentValidateRequest.md)|  | 

### Return type

[**DocumentValidateResponse**](DocumentValidateResponse.md)

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

# **void_document_api_v1_documents_document_id_void_post**
> DocumentResponse void_document_api_v1_documents_document_id_void_post(document_id)

Void Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_response import DocumentResponse
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
    api_instance = invoicepdfs.DocumentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # Void Document
        api_response = api_instance.void_document_api_v1_documents_document_id_void_post(document_id)
        print("The response of DocumentsApi->void_document_api_v1_documents_document_id_void_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->void_document_api_v1_documents_document_id_void_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

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

