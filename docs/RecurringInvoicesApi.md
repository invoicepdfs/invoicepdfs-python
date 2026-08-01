# invoicepdfs.RecurringInvoicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete**](RecurringInvoicesApi.md#cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete) | **DELETE** /api/v1/recurring-invoices/{recurring_id} | Cancel Recurring Invoice
[**create_recurring_invoice_api_v1_recurring_invoices_post**](RecurringInvoicesApi.md#create_recurring_invoice_api_v1_recurring_invoices_post) | **POST** /api/v1/recurring-invoices | Create Recurring Invoice
[**get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get**](RecurringInvoicesApi.md#get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get) | **GET** /api/v1/recurring-invoices/{recurring_id} | Get Recurring Invoice
[**list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get**](RecurringInvoicesApi.md#list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get) | **GET** /api/v1/recurring-invoices/{recurring_id}/invoices | List Generated Invoices
[**list_recurring_invoices_api_v1_recurring_invoices_get**](RecurringInvoicesApi.md#list_recurring_invoices_api_v1_recurring_invoices_get) | **GET** /api/v1/recurring-invoices | List Recurring Invoices
[**patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch**](RecurringInvoicesApi.md#patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch) | **PATCH** /api/v1/recurring-invoices/{recurring_id} | Patch Recurring Invoice
[**pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post**](RecurringInvoicesApi.md#pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post) | **POST** /api/v1/recurring-invoices/{recurring_id}/pause | Pause Recurring Invoice
[**resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post**](RecurringInvoicesApi.md#resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post) | **POST** /api/v1/recurring-invoices/{recurring_id}/resume | Resume Recurring Invoice


# **cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete**
> RecurringInvoiceResponse cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete(recurring_id)

Cancel Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 

    try:
        # Cancel Recurring Invoice
        api_response = api_instance.cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete(recurring_id)
        print("The response of RecurringInvoicesApi->cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->cancel_recurring_invoice_api_v1_recurring_invoices_recurring_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

# **create_recurring_invoice_api_v1_recurring_invoices_post**
> RecurringInvoiceResponse create_recurring_invoice_api_v1_recurring_invoices_post(recurring_invoice_create_request)

Create Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_create_request import RecurringInvoiceCreateRequest
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_invoice_create_request = invoicepdfs.RecurringInvoiceCreateRequest() # RecurringInvoiceCreateRequest | 

    try:
        # Create Recurring Invoice
        api_response = api_instance.create_recurring_invoice_api_v1_recurring_invoices_post(recurring_invoice_create_request)
        print("The response of RecurringInvoicesApi->create_recurring_invoice_api_v1_recurring_invoices_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->create_recurring_invoice_api_v1_recurring_invoices_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_invoice_create_request** | [**RecurringInvoiceCreateRequest**](RecurringInvoiceCreateRequest.md)|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

# **get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get**
> RecurringInvoiceResponse get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get(recurring_id)

Get Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 

    try:
        # Get Recurring Invoice
        api_response = api_instance.get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get(recurring_id)
        print("The response of RecurringInvoicesApi->get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->get_recurring_invoice_api_v1_recurring_invoices_recurring_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

# **list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get**
> InvoicesListResponse list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get(recurring_id, limit=limit, cursor=cursor)

List Generated Invoices

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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Generated Invoices
        api_response = api_instance.list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get(recurring_id, limit=limit, cursor=cursor)
        print("The response of RecurringInvoicesApi->list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->list_generated_invoices_api_v1_recurring_invoices_recurring_id_invoices_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

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

# **list_recurring_invoices_api_v1_recurring_invoices_get**
> RecurringInvoicesListResponse list_recurring_invoices_api_v1_recurring_invoices_get(limit=limit, cursor=cursor, status=status)

List Recurring Invoices

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoices_list_response import RecurringInvoicesListResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)
    status = 'status_example' # str |  (optional)

    try:
        # List Recurring Invoices
        api_response = api_instance.list_recurring_invoices_api_v1_recurring_invoices_get(limit=limit, cursor=cursor, status=status)
        print("The response of RecurringInvoicesApi->list_recurring_invoices_api_v1_recurring_invoices_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->list_recurring_invoices_api_v1_recurring_invoices_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 

### Return type

[**RecurringInvoicesListResponse**](RecurringInvoicesListResponse.md)

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

# **patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch**
> RecurringInvoiceResponse patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch(recurring_id, recurring_invoice_patch_request)

Patch Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_patch_request import RecurringInvoicePatchRequest
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 
    recurring_invoice_patch_request = invoicepdfs.RecurringInvoicePatchRequest() # RecurringInvoicePatchRequest | 

    try:
        # Patch Recurring Invoice
        api_response = api_instance.patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch(recurring_id, recurring_invoice_patch_request)
        print("The response of RecurringInvoicesApi->patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->patch_recurring_invoice_api_v1_recurring_invoices_recurring_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 
 **recurring_invoice_patch_request** | [**RecurringInvoicePatchRequest**](RecurringInvoicePatchRequest.md)|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

# **pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post**
> RecurringInvoiceResponse pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post(recurring_id)

Pause Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 

    try:
        # Pause Recurring Invoice
        api_response = api_instance.pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post(recurring_id)
        print("The response of RecurringInvoicesApi->pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->pause_recurring_invoice_api_v1_recurring_invoices_recurring_id_pause_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

# **resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post**
> RecurringInvoiceResponse resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post(recurring_id)

Resume Recurring Invoice

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.recurring_invoice_response import RecurringInvoiceResponse
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
    api_instance = invoicepdfs.RecurringInvoicesApi(api_client)
    recurring_id = 'recurring_id_example' # str | 

    try:
        # Resume Recurring Invoice
        api_response = api_instance.resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post(recurring_id)
        print("The response of RecurringInvoicesApi->resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecurringInvoicesApi->resume_recurring_invoice_api_v1_recurring_invoices_recurring_id_resume_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurring_id** | **str**|  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

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

