# invoicepdfs.CreditNotesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_credit_note_api_v1_credit_notes_post**](CreditNotesApi.md#create_credit_note_api_v1_credit_notes_post) | **POST** /api/v1/credit-notes | Create Credit Note
[**finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post**](CreditNotesApi.md#finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post) | **POST** /api/v1/credit-notes/{credit_note_id}/finalize | Finalize Credit Note
[**get_credit_note_api_v1_credit_notes_credit_note_id_get**](CreditNotesApi.md#get_credit_note_api_v1_credit_notes_credit_note_id_get) | **GET** /api/v1/credit-notes/{credit_note_id} | Get Credit Note
[**list_credit_notes_api_v1_credit_notes_get**](CreditNotesApi.md#list_credit_notes_api_v1_credit_notes_get) | **GET** /api/v1/credit-notes | List Credit Notes
[**render_credit_note_api_v1_credit_notes_credit_note_id_renders_post**](CreditNotesApi.md#render_credit_note_api_v1_credit_notes_credit_note_id_renders_post) | **POST** /api/v1/credit-notes/{credit_note_id}/renders | Render Credit Note


# **create_credit_note_api_v1_credit_notes_post**
> CreditNoteResponse create_credit_note_api_v1_credit_notes_post(credit_note_create_request)

Create Credit Note

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.credit_note_create_request import CreditNoteCreateRequest
from invoicepdfs.models.credit_note_response import CreditNoteResponse
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
    api_instance = invoicepdfs.CreditNotesApi(api_client)
    credit_note_create_request = invoicepdfs.CreditNoteCreateRequest() # CreditNoteCreateRequest | 

    try:
        # Create Credit Note
        api_response = api_instance.create_credit_note_api_v1_credit_notes_post(credit_note_create_request)
        print("The response of CreditNotesApi->create_credit_note_api_v1_credit_notes_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CreditNotesApi->create_credit_note_api_v1_credit_notes_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credit_note_create_request** | [**CreditNoteCreateRequest**](CreditNoteCreateRequest.md)|  | 

### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

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

# **finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post**
> CreditNoteResponse finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post(credit_note_id)

Finalize Credit Note

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.credit_note_response import CreditNoteResponse
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
    api_instance = invoicepdfs.CreditNotesApi(api_client)
    credit_note_id = 'credit_note_id_example' # str | 

    try:
        # Finalize Credit Note
        api_response = api_instance.finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post(credit_note_id)
        print("The response of CreditNotesApi->finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CreditNotesApi->finalize_credit_note_api_v1_credit_notes_credit_note_id_finalize_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credit_note_id** | **str**|  | 

### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

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

# **get_credit_note_api_v1_credit_notes_credit_note_id_get**
> CreditNoteResponse get_credit_note_api_v1_credit_notes_credit_note_id_get(credit_note_id)

Get Credit Note

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.credit_note_response import CreditNoteResponse
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
    api_instance = invoicepdfs.CreditNotesApi(api_client)
    credit_note_id = 'credit_note_id_example' # str | 

    try:
        # Get Credit Note
        api_response = api_instance.get_credit_note_api_v1_credit_notes_credit_note_id_get(credit_note_id)
        print("The response of CreditNotesApi->get_credit_note_api_v1_credit_notes_credit_note_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CreditNotesApi->get_credit_note_api_v1_credit_notes_credit_note_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credit_note_id** | **str**|  | 

### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

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

# **list_credit_notes_api_v1_credit_notes_get**
> CreditNotesListResponse list_credit_notes_api_v1_credit_notes_get(limit=limit, cursor=cursor)

List Credit Notes

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.credit_notes_list_response import CreditNotesListResponse
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
    api_instance = invoicepdfs.CreditNotesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Credit Notes
        api_response = api_instance.list_credit_notes_api_v1_credit_notes_get(limit=limit, cursor=cursor)
        print("The response of CreditNotesApi->list_credit_notes_api_v1_credit_notes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CreditNotesApi->list_credit_notes_api_v1_credit_notes_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**CreditNotesListResponse**](CreditNotesListResponse.md)

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

# **render_credit_note_api_v1_credit_notes_credit_note_id_renders_post**
> object render_credit_note_api_v1_credit_notes_credit_note_id_renders_post(credit_note_id, credit_note_render_request=credit_note_render_request)

Render Credit Note

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.credit_note_render_request import CreditNoteRenderRequest
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
    api_instance = invoicepdfs.CreditNotesApi(api_client)
    credit_note_id = 'credit_note_id_example' # str | 
    credit_note_render_request = invoicepdfs.CreditNoteRenderRequest() # CreditNoteRenderRequest |  (optional)

    try:
        # Render Credit Note
        api_response = api_instance.render_credit_note_api_v1_credit_notes_credit_note_id_renders_post(credit_note_id, credit_note_render_request=credit_note_render_request)
        print("The response of CreditNotesApi->render_credit_note_api_v1_credit_notes_credit_note_id_renders_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CreditNotesApi->render_credit_note_api_v1_credit_notes_credit_note_id_renders_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credit_note_id** | **str**|  | 
 **credit_note_render_request** | [**CreditNoteRenderRequest**](CreditNoteRenderRequest.md)|  | [optional] 

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

