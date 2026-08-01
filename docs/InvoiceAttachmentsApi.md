# invoicepdfs.InvoiceAttachmentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_attachment_api_v1_documents_invoice_id_attachments_post**](InvoiceAttachmentsApi.md#create_attachment_api_v1_documents_invoice_id_attachments_post) | **POST** /api/v1/documents/{invoice_id}/attachments | Create Attachment
[**delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete**](InvoiceAttachmentsApi.md#delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete) | **DELETE** /api/v1/documents/{invoice_id}/attachments/{attachment_id} | Delete Attachment
[**list_attachments_api_v1_documents_invoice_id_attachments_get**](InvoiceAttachmentsApi.md#list_attachments_api_v1_documents_invoice_id_attachments_get) | **GET** /api/v1/documents/{invoice_id}/attachments | List Attachments


# **create_attachment_api_v1_documents_invoice_id_attachments_post**
> InvoiceAttachmentResponse create_attachment_api_v1_documents_invoice_id_attachments_post(invoice_id, invoice_attachment_create_request)

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
    api_instance = invoicepdfs.InvoiceAttachmentsApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    invoice_attachment_create_request = invoicepdfs.InvoiceAttachmentCreateRequest() # InvoiceAttachmentCreateRequest | 

    try:
        # Create Attachment
        api_response = api_instance.create_attachment_api_v1_documents_invoice_id_attachments_post(invoice_id, invoice_attachment_create_request)
        print("The response of InvoiceAttachmentsApi->create_attachment_api_v1_documents_invoice_id_attachments_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceAttachmentsApi->create_attachment_api_v1_documents_invoice_id_attachments_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
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

# **delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete**
> SimpleBoolResponse delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete(invoice_id, attachment_id)

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
    api_instance = invoicepdfs.InvoiceAttachmentsApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    attachment_id = 'attachment_id_example' # str | 

    try:
        # Delete Attachment
        api_response = api_instance.delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete(invoice_id, attachment_id)
        print("The response of InvoiceAttachmentsApi->delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceAttachmentsApi->delete_attachment_api_v1_documents_invoice_id_attachments_attachment_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
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

# **list_attachments_api_v1_documents_invoice_id_attachments_get**
> InvoiceAttachmentsListResponse list_attachments_api_v1_documents_invoice_id_attachments_get(invoice_id)

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
    api_instance = invoicepdfs.InvoiceAttachmentsApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # List Attachments
        api_response = api_instance.list_attachments_api_v1_documents_invoice_id_attachments_get(invoice_id)
        print("The response of InvoiceAttachmentsApi->list_attachments_api_v1_documents_invoice_id_attachments_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoiceAttachmentsApi->list_attachments_api_v1_documents_invoice_id_attachments_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

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

