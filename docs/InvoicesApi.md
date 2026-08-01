# invoicepdfs.InvoicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**archive_invoice_api_v1_invoices_invoice_id_archive_post**](InvoicesApi.md#archive_invoice_api_v1_invoices_invoice_id_archive_post) | **POST** /api/v1/invoices/{invoice_id}/archive | Archive Invoice
[**calculate_invoice_api_v1_invoices_calculate_post**](InvoicesApi.md#calculate_invoice_api_v1_invoices_calculate_post) | **POST** /api/v1/invoices/calculate | Calculate Invoice
[**create_invoice_api_v1_invoices_post**](InvoicesApi.md#create_invoice_api_v1_invoices_post) | **POST** /api/v1/invoices | Create Invoice
[**delete_invoice_api_v1_invoices_invoice_id_delete**](InvoicesApi.md#delete_invoice_api_v1_invoices_invoice_id_delete) | **DELETE** /api/v1/invoices/{invoice_id} | Delete Invoice
[**duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post**](InvoicesApi.md#duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post) | **POST** /api/v1/invoices/{invoice_id}/duplicate | Duplicate Invoice
[**finalize_invoice_api_v1_invoices_invoice_id_finalize_post**](InvoicesApi.md#finalize_invoice_api_v1_invoices_invoice_id_finalize_post) | **POST** /api/v1/invoices/{invoice_id}/finalize | Finalize Invoice
[**get_invoice_api_v1_invoices_invoice_id_get**](InvoicesApi.md#get_invoice_api_v1_invoices_invoice_id_get) | **GET** /api/v1/invoices/{invoice_id} | Get Invoice
[**list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get**](InvoicesApi.md#list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get) | **GET** /api/v1/invoices/{invoice_id}/deliveries | List Invoice Deliveries
[**list_invoices_api_v1_invoices_get**](InvoicesApi.md#list_invoices_api_v1_invoices_get) | **GET** /api/v1/invoices | List Invoices
[**mark_paid_api_v1_invoices_invoice_id_mark_paid_post**](InvoicesApi.md#mark_paid_api_v1_invoices_invoice_id_mark_paid_post) | **POST** /api/v1/invoices/{invoice_id}/mark-paid | Mark Paid
[**mark_sent_api_v1_invoices_invoice_id_mark_sent_post**](InvoicesApi.md#mark_sent_api_v1_invoices_invoice_id_mark_sent_post) | **POST** /api/v1/invoices/{invoice_id}/mark-sent | Mark Sent
[**mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post**](InvoicesApi.md#mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post) | **POST** /api/v1/invoices/{invoice_id}/mark-unpaid | Mark Unpaid
[**patch_invoice_api_v1_invoices_invoice_id_patch**](InvoicesApi.md#patch_invoice_api_v1_invoices_invoice_id_patch) | **PATCH** /api/v1/invoices/{invoice_id} | Patch Invoice
[**preview_invoice_api_v1_invoices_preview_post**](InvoicesApi.md#preview_invoice_api_v1_invoices_preview_post) | **POST** /api/v1/invoices/preview | Preview Invoice
[**render_invoice_api_v1_invoices_invoice_id_renders_post**](InvoicesApi.md#render_invoice_api_v1_invoices_invoice_id_renders_post) | **POST** /api/v1/invoices/{invoice_id}/renders | Render Invoice
[**replace_invoice_api_v1_invoices_invoice_id_put**](InvoicesApi.md#replace_invoice_api_v1_invoices_invoice_id_put) | **PUT** /api/v1/invoices/{invoice_id} | Replace Invoice
[**restore_invoice_api_v1_invoices_invoice_id_restore_post**](InvoicesApi.md#restore_invoice_api_v1_invoices_invoice_id_restore_post) | **POST** /api/v1/invoices/{invoice_id}/restore | Restore Invoice
[**send_invoice_api_v1_invoices_invoice_id_send_post**](InvoicesApi.md#send_invoice_api_v1_invoices_invoice_id_send_post) | **POST** /api/v1/invoices/{invoice_id}/send | Send Invoice
[**validate_invoice_api_v1_invoices_validate_post**](InvoicesApi.md#validate_invoice_api_v1_invoices_validate_post) | **POST** /api/v1/invoices/validate | Validate Invoice
[**void_invoice_api_v1_invoices_invoice_id_void_post**](InvoicesApi.md#void_invoice_api_v1_invoices_invoice_id_void_post) | **POST** /api/v1/invoices/{invoice_id}/void | Void Invoice


# **archive_invoice_api_v1_invoices_invoice_id_archive_post**
> InvoiceResponse archive_invoice_api_v1_invoices_invoice_id_archive_post(invoice_id)

Archive Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Archive Invoice
        api_response = api_instance.archive_invoice_api_v1_invoices_invoice_id_archive_post(invoice_id)
        print("The response of InvoicesApi->archive_invoice_api_v1_invoices_invoice_id_archive_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->archive_invoice_api_v1_invoices_invoice_id_archive_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **calculate_invoice_api_v1_invoices_calculate_post**
> Dict[str, object] calculate_invoice_api_v1_invoices_calculate_post(invoice_draft_request)

Calculate Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_draft_request import InvoiceDraftRequest
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_draft_request = invoicepdfs.InvoiceDraftRequest() # InvoiceDraftRequest | 

    try:
        # Calculate Invoice
        api_response = api_instance.calculate_invoice_api_v1_invoices_calculate_post(invoice_draft_request)
        print("The response of InvoicesApi->calculate_invoice_api_v1_invoices_calculate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->calculate_invoice_api_v1_invoices_calculate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_draft_request** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md)|  | 

### Return type

**Dict[str, object]**

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

# **create_invoice_api_v1_invoices_post**
> InvoiceResponse create_invoice_api_v1_invoices_post(invoice_create_request, idempotency_key=idempotency_key)

Create Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_create_request import InvoiceCreateRequest
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_create_request = invoicepdfs.InvoiceCreateRequest() # InvoiceCreateRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Invoice
        api_response = api_instance.create_invoice_api_v1_invoices_post(invoice_create_request, idempotency_key=idempotency_key)
        print("The response of InvoicesApi->create_invoice_api_v1_invoices_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->create_invoice_api_v1_invoices_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_create_request** | [**InvoiceCreateRequest**](InvoiceCreateRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **delete_invoice_api_v1_invoices_invoice_id_delete**
> SimpleBoolResponse delete_invoice_api_v1_invoices_invoice_id_delete(invoice_id)

Delete Invoice

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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Delete Invoice
        api_response = api_instance.delete_invoice_api_v1_invoices_invoice_id_delete(invoice_id)
        print("The response of InvoicesApi->delete_invoice_api_v1_invoices_invoice_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->delete_invoice_api_v1_invoices_invoice_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

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

# **duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post**
> InvoiceResponse duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post(invoice_id)

Duplicate Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Duplicate Invoice
        api_response = api_instance.duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post(invoice_id)
        print("The response of InvoicesApi->duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->duplicate_invoice_api_v1_invoices_invoice_id_duplicate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **finalize_invoice_api_v1_invoices_invoice_id_finalize_post**
> Dict[str, object] finalize_invoice_api_v1_invoices_invoice_id_finalize_post(invoice_id, idempotency_key=idempotency_key)

Finalize Invoice

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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Finalize Invoice
        api_response = api_instance.finalize_invoice_api_v1_invoices_invoice_id_finalize_post(invoice_id, idempotency_key=idempotency_key)
        print("The response of InvoicesApi->finalize_invoice_api_v1_invoices_invoice_id_finalize_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->finalize_invoice_api_v1_invoices_invoice_id_finalize_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **idempotency_key** | **str**|  | [optional] 

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

# **get_invoice_api_v1_invoices_invoice_id_get**
> InvoiceResponse get_invoice_api_v1_invoices_invoice_id_get(invoice_id)

Get Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Get Invoice
        api_response = api_instance.get_invoice_api_v1_invoices_invoice_id_get(invoice_id)
        print("The response of InvoicesApi->get_invoice_api_v1_invoices_invoice_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->get_invoice_api_v1_invoices_invoice_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get**
> DeliveriesListResponse list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get(invoice_id, limit=limit, cursor=cursor)

List Invoice Deliveries

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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Invoice Deliveries
        api_response = api_instance.list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get(invoice_id, limit=limit, cursor=cursor)
        print("The response of InvoicesApi->list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->list_invoice_deliveries_api_v1_invoices_invoice_id_deliveries_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
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

# **list_invoices_api_v1_invoices_get**
> InvoicesListResponse list_invoices_api_v1_invoices_get(limit=limit, cursor=cursor, status=status)

List Invoices

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoices_list_response import InvoicesListResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)
    status = 'status_example' # str |  (optional)

    try:
        # List Invoices
        api_response = api_instance.list_invoices_api_v1_invoices_get(limit=limit, cursor=cursor, status=status)
        print("The response of InvoicesApi->list_invoices_api_v1_invoices_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->list_invoices_api_v1_invoices_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 

### Return type

[**InvoicesListResponse**](InvoicesListResponse.md)

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

# **mark_paid_api_v1_invoices_invoice_id_mark_paid_post**
> InvoiceResponse mark_paid_api_v1_invoices_invoice_id_mark_paid_post(invoice_id)

Mark Paid

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Mark Paid
        api_response = api_instance.mark_paid_api_v1_invoices_invoice_id_mark_paid_post(invoice_id)
        print("The response of InvoicesApi->mark_paid_api_v1_invoices_invoice_id_mark_paid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->mark_paid_api_v1_invoices_invoice_id_mark_paid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **mark_sent_api_v1_invoices_invoice_id_mark_sent_post**
> InvoiceResponse mark_sent_api_v1_invoices_invoice_id_mark_sent_post(invoice_id)

Mark Sent

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Mark Sent
        api_response = api_instance.mark_sent_api_v1_invoices_invoice_id_mark_sent_post(invoice_id)
        print("The response of InvoicesApi->mark_sent_api_v1_invoices_invoice_id_mark_sent_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->mark_sent_api_v1_invoices_invoice_id_mark_sent_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post**
> InvoiceResponse mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post(invoice_id)

Mark Unpaid

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Mark Unpaid
        api_response = api_instance.mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post(invoice_id)
        print("The response of InvoicesApi->mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->mark_unpaid_api_v1_invoices_invoice_id_mark_unpaid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **patch_invoice_api_v1_invoices_invoice_id_patch**
> InvoiceResponse patch_invoice_api_v1_invoices_invoice_id_patch(invoice_id, invoice_patch_request, idempotency_key=idempotency_key)

Patch Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_patch_request import InvoicePatchRequest
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    invoice_patch_request = invoicepdfs.InvoicePatchRequest() # InvoicePatchRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Patch Invoice
        api_response = api_instance.patch_invoice_api_v1_invoices_invoice_id_patch(invoice_id, invoice_patch_request, idempotency_key=idempotency_key)
        print("The response of InvoicesApi->patch_invoice_api_v1_invoices_invoice_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->patch_invoice_api_v1_invoices_invoice_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **invoice_patch_request** | [**InvoicePatchRequest**](InvoicePatchRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **preview_invoice_api_v1_invoices_preview_post**
> object preview_invoice_api_v1_invoices_preview_post(invoice_preview_request)

Preview Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_preview_request import InvoicePreviewRequest
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_preview_request = invoicepdfs.InvoicePreviewRequest() # InvoicePreviewRequest | 

    try:
        # Preview Invoice
        api_response = api_instance.preview_invoice_api_v1_invoices_preview_post(invoice_preview_request)
        print("The response of InvoicesApi->preview_invoice_api_v1_invoices_preview_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->preview_invoice_api_v1_invoices_preview_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_preview_request** | [**InvoicePreviewRequest**](InvoicePreviewRequest.md)|  | 

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

# **render_invoice_api_v1_invoices_invoice_id_renders_post**
> object render_invoice_api_v1_invoices_invoice_id_renders_post(invoice_id, invoice_render_request, idempotency_key=idempotency_key)

Render Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_render_request import InvoiceRenderRequest
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    invoice_render_request = invoicepdfs.InvoiceRenderRequest() # InvoiceRenderRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Render Invoice
        api_response = api_instance.render_invoice_api_v1_invoices_invoice_id_renders_post(invoice_id, invoice_render_request, idempotency_key=idempotency_key)
        print("The response of InvoicesApi->render_invoice_api_v1_invoices_invoice_id_renders_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->render_invoice_api_v1_invoices_invoice_id_renders_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **invoice_render_request** | [**InvoiceRenderRequest**](InvoiceRenderRequest.md)|  | 
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

# **replace_invoice_api_v1_invoices_invoice_id_put**
> InvoiceResponse replace_invoice_api_v1_invoices_invoice_id_put(invoice_id, invoice_create_request, idempotency_key=idempotency_key)

Replace Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_create_request import InvoiceCreateRequest
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    invoice_create_request = invoicepdfs.InvoiceCreateRequest() # InvoiceCreateRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Replace Invoice
        api_response = api_instance.replace_invoice_api_v1_invoices_invoice_id_put(invoice_id, invoice_create_request, idempotency_key=idempotency_key)
        print("The response of InvoicesApi->replace_invoice_api_v1_invoices_invoice_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->replace_invoice_api_v1_invoices_invoice_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **invoice_create_request** | [**InvoiceCreateRequest**](InvoiceCreateRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **restore_invoice_api_v1_invoices_invoice_id_restore_post**
> InvoiceResponse restore_invoice_api_v1_invoices_invoice_id_restore_post(invoice_id)

Restore Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Restore Invoice
        api_response = api_instance.restore_invoice_api_v1_invoices_invoice_id_restore_post(invoice_id)
        print("The response of InvoicesApi->restore_invoice_api_v1_invoices_invoice_id_restore_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->restore_invoice_api_v1_invoices_invoice_id_restore_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

# **send_invoice_api_v1_invoices_invoice_id_send_post**
> DeliveryResponse send_invoice_api_v1_invoices_invoice_id_send_post(invoice_id, delivery_send_request)

Send Invoice

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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    delivery_send_request = invoicepdfs.DeliverySendRequest() # DeliverySendRequest | 

    try:
        # Send Invoice
        api_response = api_instance.send_invoice_api_v1_invoices_invoice_id_send_post(invoice_id, delivery_send_request)
        print("The response of InvoicesApi->send_invoice_api_v1_invoices_invoice_id_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->send_invoice_api_v1_invoices_invoice_id_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
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

# **validate_invoice_api_v1_invoices_validate_post**
> Dict[str, object] validate_invoice_api_v1_invoices_validate_post(invoice_draft_request)

Validate Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_draft_request import InvoiceDraftRequest
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_draft_request = invoicepdfs.InvoiceDraftRequest() # InvoiceDraftRequest | 

    try:
        # Validate Invoice
        api_response = api_instance.validate_invoice_api_v1_invoices_validate_post(invoice_draft_request)
        print("The response of InvoicesApi->validate_invoice_api_v1_invoices_validate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->validate_invoice_api_v1_invoices_validate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_draft_request** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md)|  | 

### Return type

**Dict[str, object]**

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

# **void_invoice_api_v1_invoices_invoice_id_void_post**
> InvoiceResponse void_invoice_api_v1_invoices_invoice_id_void_post(invoice_id)

Void Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.invoice_response import InvoiceResponse
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
    api_instance = invoicepdfs.InvoicesApi(api_client)
    invoice_id = 'invoice_id_example' # str | 

    try:
        # Void Invoice
        api_response = api_instance.void_invoice_api_v1_invoices_invoice_id_void_post(invoice_id)
        print("The response of InvoicesApi->void_invoice_api_v1_invoices_invoice_id_void_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->void_invoice_api_v1_invoices_invoice_id_void_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

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

