# invoicepdfs.PaymentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_api_v1_invoices_invoice_id_payments_post**](PaymentsApi.md#create_payment_api_v1_invoices_invoice_id_payments_post) | **POST** /api/v1/invoices/{invoice_id}/payments | Create Payment
[**delete_payment_api_v1_payments_payment_id_delete**](PaymentsApi.md#delete_payment_api_v1_payments_payment_id_delete) | **DELETE** /api/v1/payments/{payment_id} | Delete Payment
[**get_payment_api_v1_payments_payment_id_get**](PaymentsApi.md#get_payment_api_v1_payments_payment_id_get) | **GET** /api/v1/payments/{payment_id} | Get Payment
[**list_invoice_payments_api_v1_invoices_invoice_id_payments_get**](PaymentsApi.md#list_invoice_payments_api_v1_invoices_invoice_id_payments_get) | **GET** /api/v1/invoices/{invoice_id}/payments | List Invoice Payments
[**update_payment_api_v1_payments_payment_id_patch**](PaymentsApi.md#update_payment_api_v1_payments_payment_id_patch) | **PATCH** /api/v1/payments/{payment_id} | Update Payment


# **create_payment_api_v1_invoices_invoice_id_payments_post**
> PaymentResponse create_payment_api_v1_invoices_invoice_id_payments_post(invoice_id, payment_create_request)

Create Payment

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.payment_create_request import PaymentCreateRequest
from invoicepdfs.models.payment_response import PaymentResponse
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
    api_instance = invoicepdfs.PaymentsApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    payment_create_request = invoicepdfs.PaymentCreateRequest() # PaymentCreateRequest | 

    try:
        # Create Payment
        api_response = api_instance.create_payment_api_v1_invoices_invoice_id_payments_post(invoice_id, payment_create_request)
        print("The response of PaymentsApi->create_payment_api_v1_invoices_invoice_id_payments_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->create_payment_api_v1_invoices_invoice_id_payments_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **payment_create_request** | [**PaymentCreateRequest**](PaymentCreateRequest.md)|  | 

### Return type

[**PaymentResponse**](PaymentResponse.md)

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

# **delete_payment_api_v1_payments_payment_id_delete**
> SimpleBoolResponse delete_payment_api_v1_payments_payment_id_delete(payment_id)

Delete Payment

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
    api_instance = invoicepdfs.PaymentsApi(api_client)
    payment_id = 'payment_id_example' # str | 

    try:
        # Delete Payment
        api_response = api_instance.delete_payment_api_v1_payments_payment_id_delete(payment_id)
        print("The response of PaymentsApi->delete_payment_api_v1_payments_payment_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->delete_payment_api_v1_payments_payment_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_id** | **str**|  | 

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

# **get_payment_api_v1_payments_payment_id_get**
> PaymentResponse get_payment_api_v1_payments_payment_id_get(payment_id)

Get Payment

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.payment_response import PaymentResponse
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
    api_instance = invoicepdfs.PaymentsApi(api_client)
    payment_id = 'payment_id_example' # str | 

    try:
        # Get Payment
        api_response = api_instance.get_payment_api_v1_payments_payment_id_get(payment_id)
        print("The response of PaymentsApi->get_payment_api_v1_payments_payment_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->get_payment_api_v1_payments_payment_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_id** | **str**|  | 

### Return type

[**PaymentResponse**](PaymentResponse.md)

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

# **list_invoice_payments_api_v1_invoices_invoice_id_payments_get**
> PaymentsListResponse list_invoice_payments_api_v1_invoices_invoice_id_payments_get(invoice_id, limit=limit, cursor=cursor)

List Invoice Payments

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.payments_list_response import PaymentsListResponse
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
    api_instance = invoicepdfs.PaymentsApi(api_client)
    invoice_id = 'invoice_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Invoice Payments
        api_response = api_instance.list_invoice_payments_api_v1_invoices_invoice_id_payments_get(invoice_id, limit=limit, cursor=cursor)
        print("The response of PaymentsApi->list_invoice_payments_api_v1_invoices_invoice_id_payments_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->list_invoice_payments_api_v1_invoices_invoice_id_payments_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**PaymentsListResponse**](PaymentsListResponse.md)

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

# **update_payment_api_v1_payments_payment_id_patch**
> PaymentResponse update_payment_api_v1_payments_payment_id_patch(payment_id, payment_patch_request)

Update Payment

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.payment_patch_request import PaymentPatchRequest
from invoicepdfs.models.payment_response import PaymentResponse
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
    api_instance = invoicepdfs.PaymentsApi(api_client)
    payment_id = 'payment_id_example' # str | 
    payment_patch_request = invoicepdfs.PaymentPatchRequest() # PaymentPatchRequest | 

    try:
        # Update Payment
        api_response = api_instance.update_payment_api_v1_payments_payment_id_patch(payment_id, payment_patch_request)
        print("The response of PaymentsApi->update_payment_api_v1_payments_payment_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->update_payment_api_v1_payments_payment_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_id** | **str**|  | 
 **payment_patch_request** | [**PaymentPatchRequest**](PaymentPatchRequest.md)|  | 

### Return type

[**PaymentResponse**](PaymentResponse.md)

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

