# invoicepdfs.DocumentAttachmentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_document_attachment**](DocumentAttachmentsApi.md#create_document_attachment) | **POST** /api/v1/documents/{document_id}/attachments | Create Attachment
[**delete_document_attachment**](DocumentAttachmentsApi.md#delete_document_attachment) | **DELETE** /api/v1/documents/{document_id}/attachments/{attachment_id} | Delete Attachment
[**list_document_attachments**](DocumentAttachmentsApi.md#list_document_attachments) | **GET** /api/v1/documents/{document_id}/attachments | List Attachments


# **create_document_attachment**
> InvoiceAttachmentResponse create_document_attachment(document_id, invoice_attachment_create_request)

Create Attachment

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_attachment_create_request import InvoiceAttachmentCreateRequest
from invoicepdfs.models.invoice_attachment_response import InvoiceAttachmentResponse
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
    api_instance = invoicepdfs.DocumentAttachmentsApi(api_client)
    document_id = 'document_id_example' # str | 
    invoice_attachment_create_request = invoicepdfs.InvoiceAttachmentCreateRequest() # InvoiceAttachmentCreateRequest | 

    try:
        # Create Attachment
        api_response = api_instance.create_document_attachment(document_id, invoice_attachment_create_request)
        print("The response of DocumentAttachmentsApi->create_document_attachment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentAttachmentsApi->create_document_attachment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **invoice_attachment_create_request** | [**InvoiceAttachmentCreateRequest**](InvoiceAttachmentCreateRequest.md)|  | 

### Return type

[**InvoiceAttachmentResponse**](InvoiceAttachmentResponse.md)

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

# **delete_document_attachment**
> SimpleBoolResponse delete_document_attachment(document_id, attachment_id)

Delete Attachment

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
    api_instance = invoicepdfs.DocumentAttachmentsApi(api_client)
    document_id = 'document_id_example' # str | 
    attachment_id = 'attachment_id_example' # str | 

    try:
        # Delete Attachment
        api_response = api_instance.delete_document_attachment(document_id, attachment_id)
        print("The response of DocumentAttachmentsApi->delete_document_attachment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentAttachmentsApi->delete_document_attachment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **attachment_id** | **str**|  | 

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

# **list_document_attachments**
> InvoiceAttachmentsListResponse list_document_attachments(document_id)

List Attachments

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_attachments_list_response import InvoiceAttachmentsListResponse
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
    api_instance = invoicepdfs.DocumentAttachmentsApi(api_client)
    document_id = 'document_id_example' # str | 

    try:
        # List Attachments
        api_response = api_instance.list_document_attachments(document_id)
        print("The response of DocumentAttachmentsApi->list_document_attachments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DocumentAttachmentsApi->list_document_attachments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 

### Return type

[**InvoiceAttachmentsListResponse**](InvoiceAttachmentsListResponse.md)

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

