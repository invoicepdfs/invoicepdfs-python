# invoicepdfs.DocumentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_document_api_v1_documents_calculate_post**](DocumentsApi.md#calculate_document_api_v1_documents_calculate_post) | **POST** /api/v1/documents/calculate | Calculate Document
[**render_document_api_v1_documents_render_post**](DocumentsApi.md#render_document_api_v1_documents_render_post) | **POST** /api/v1/documents/render | Render Document
[**validate_document_api_v1_documents_validate_post**](DocumentsApi.md#validate_document_api_v1_documents_validate_post) | **POST** /api/v1/documents/validate | Validate Document


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

# **render_document_api_v1_documents_render_post**
> object render_document_api_v1_documents_render_post(document_render_request, idempotency_key=idempotency_key)

Render Document

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_render_request import DocumentRenderRequest
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
    document_render_request = invoicepdfs.DocumentRenderRequest() # DocumentRenderRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Render Document
        api_response = api_instance.render_document_api_v1_documents_render_post(document_render_request, idempotency_key=idempotency_key)
        print("The response of DocumentsApi->render_document_api_v1_documents_render_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentsApi->render_document_api_v1_documents_render_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_render_request** | [**DocumentRenderRequest**](DocumentRenderRequest.md)|  | 
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

