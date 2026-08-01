# invoicepdfs.NumberingSequencesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**consume_next_api_v1_numbering_sequences_sequence_id_next_post**](NumberingSequencesApi.md#consume_next_api_v1_numbering_sequences_sequence_id_next_post) | **POST** /api/v1/numbering-sequences/{sequence_id}/next | Consume Next
[**create_sequence_api_v1_numbering_sequences_post**](NumberingSequencesApi.md#create_sequence_api_v1_numbering_sequences_post) | **POST** /api/v1/numbering-sequences | Create Sequence
[**delete_sequence_api_v1_numbering_sequences_sequence_id_delete**](NumberingSequencesApi.md#delete_sequence_api_v1_numbering_sequences_sequence_id_delete) | **DELETE** /api/v1/numbering-sequences/{sequence_id} | Delete Sequence
[**get_sequence_api_v1_numbering_sequences_sequence_id_get**](NumberingSequencesApi.md#get_sequence_api_v1_numbering_sequences_sequence_id_get) | **GET** /api/v1/numbering-sequences/{sequence_id} | Get Sequence
[**list_sequences_api_v1_numbering_sequences_get**](NumberingSequencesApi.md#list_sequences_api_v1_numbering_sequences_get) | **GET** /api/v1/numbering-sequences | List Sequences
[**preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post**](NumberingSequencesApi.md#preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post) | **POST** /api/v1/numbering-sequences/{sequence_id}/preview | Preview Sequence
[**update_sequence_api_v1_numbering_sequences_sequence_id_patch**](NumberingSequencesApi.md#update_sequence_api_v1_numbering_sequences_sequence_id_patch) | **PATCH** /api/v1/numbering-sequences/{sequence_id} | Update Sequence


# **consume_next_api_v1_numbering_sequences_sequence_id_next_post**
> NumberingSequenceResponse consume_next_api_v1_numbering_sequences_sequence_id_next_post(sequence_id)

Consume Next

Consume and return the next number, incrementing the counter.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequence_response import NumberingSequenceResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    sequence_id = 'sequence_id_example' # str | 

    try:
        # Consume Next
        api_response = api_instance.consume_next_api_v1_numbering_sequences_sequence_id_next_post(sequence_id)
        print("The response of NumberingSequencesApi->consume_next_api_v1_numbering_sequences_sequence_id_next_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->consume_next_api_v1_numbering_sequences_sequence_id_next_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sequence_id** | **str**|  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

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

# **create_sequence_api_v1_numbering_sequences_post**
> NumberingSequenceResponse create_sequence_api_v1_numbering_sequences_post(numbering_sequence_create_request)

Create Sequence

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequence_create_request import NumberingSequenceCreateRequest
from invoicepdfs.models.numbering_sequence_response import NumberingSequenceResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    numbering_sequence_create_request = invoicepdfs.NumberingSequenceCreateRequest() # NumberingSequenceCreateRequest | 

    try:
        # Create Sequence
        api_response = api_instance.create_sequence_api_v1_numbering_sequences_post(numbering_sequence_create_request)
        print("The response of NumberingSequencesApi->create_sequence_api_v1_numbering_sequences_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->create_sequence_api_v1_numbering_sequences_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **numbering_sequence_create_request** | [**NumberingSequenceCreateRequest**](NumberingSequenceCreateRequest.md)|  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

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

# **delete_sequence_api_v1_numbering_sequences_sequence_id_delete**
> SimpleBoolResponse delete_sequence_api_v1_numbering_sequences_sequence_id_delete(sequence_id)

Delete Sequence

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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    sequence_id = 'sequence_id_example' # str | 

    try:
        # Delete Sequence
        api_response = api_instance.delete_sequence_api_v1_numbering_sequences_sequence_id_delete(sequence_id)
        print("The response of NumberingSequencesApi->delete_sequence_api_v1_numbering_sequences_sequence_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->delete_sequence_api_v1_numbering_sequences_sequence_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sequence_id** | **str**|  | 

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

# **get_sequence_api_v1_numbering_sequences_sequence_id_get**
> NumberingSequenceResponse get_sequence_api_v1_numbering_sequences_sequence_id_get(sequence_id)

Get Sequence

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequence_response import NumberingSequenceResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    sequence_id = 'sequence_id_example' # str | 

    try:
        # Get Sequence
        api_response = api_instance.get_sequence_api_v1_numbering_sequences_sequence_id_get(sequence_id)
        print("The response of NumberingSequencesApi->get_sequence_api_v1_numbering_sequences_sequence_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->get_sequence_api_v1_numbering_sequences_sequence_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sequence_id** | **str**|  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

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

# **list_sequences_api_v1_numbering_sequences_get**
> NumberingSequencesListResponse list_sequences_api_v1_numbering_sequences_get(limit=limit, cursor=cursor)

List Sequences

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequences_list_response import NumberingSequencesListResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Sequences
        api_response = api_instance.list_sequences_api_v1_numbering_sequences_get(limit=limit, cursor=cursor)
        print("The response of NumberingSequencesApi->list_sequences_api_v1_numbering_sequences_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->list_sequences_api_v1_numbering_sequences_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**NumberingSequencesListResponse**](NumberingSequencesListResponse.md)

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

# **preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post**
> NumberingSequencePreviewResponse preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post(sequence_id)

Preview Sequence

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequence_preview_response import NumberingSequencePreviewResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    sequence_id = 'sequence_id_example' # str | 

    try:
        # Preview Sequence
        api_response = api_instance.preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post(sequence_id)
        print("The response of NumberingSequencesApi->preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->preview_sequence_api_v1_numbering_sequences_sequence_id_preview_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sequence_id** | **str**|  | 

### Return type

[**NumberingSequencePreviewResponse**](NumberingSequencePreviewResponse.md)

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

# **update_sequence_api_v1_numbering_sequences_sequence_id_patch**
> NumberingSequenceResponse update_sequence_api_v1_numbering_sequences_sequence_id_patch(sequence_id, numbering_sequence_patch_request)

Update Sequence

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.numbering_sequence_patch_request import NumberingSequencePatchRequest
from invoicepdfs.models.numbering_sequence_response import NumberingSequenceResponse
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
    api_instance = invoicepdfs.NumberingSequencesApi(api_client)
    sequence_id = 'sequence_id_example' # str | 
    numbering_sequence_patch_request = invoicepdfs.NumberingSequencePatchRequest() # NumberingSequencePatchRequest | 

    try:
        # Update Sequence
        api_response = api_instance.update_sequence_api_v1_numbering_sequences_sequence_id_patch(sequence_id, numbering_sequence_patch_request)
        print("The response of NumberingSequencesApi->update_sequence_api_v1_numbering_sequences_sequence_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumberingSequencesApi->update_sequence_api_v1_numbering_sequences_sequence_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sequence_id** | **str**|  | 
 **numbering_sequence_patch_request** | [**NumberingSequencePatchRequest**](NumberingSequencePatchRequest.md)|  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

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

