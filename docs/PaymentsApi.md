# invoicepdfs.PaymentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_document_payment**](PaymentsApi.md#create_document_payment) | **POST** /api/v1/documents/{document_id}/payments | Create Document Payment
[**delete_payment**](PaymentsApi.md#delete_payment) | **DELETE** /api/v1/payments/{payment_id} | Delete Payment
[**get_payment**](PaymentsApi.md#get_payment) | **GET** /api/v1/payments/{payment_id} | Get Payment
[**list_document_payments**](PaymentsApi.md#list_document_payments) | **GET** /api/v1/documents/{document_id}/payments | List Document Payments
[**update_payment**](PaymentsApi.md#update_payment) | **PATCH** /api/v1/payments/{payment_id} | Update Payment


# **create_document_payment**
> PaymentResponse create_document_payment(document_id, payment_create_request)

Create Document Payment

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
    document_id = 'document_id_example' # str | 
    payment_create_request = invoicepdfs.PaymentCreateRequest() # PaymentCreateRequest | 

    try:
        # Create Document Payment
        api_response = api_instance.create_document_payment(document_id, payment_create_request)
        print("The response of PaymentsApi->create_document_payment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->create_document_payment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
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

# **delete_payment**
> SimpleBoolResponse delete_payment(payment_id)

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
        api_response = api_instance.delete_payment(payment_id)
        print("The response of PaymentsApi->delete_payment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->delete_payment: %s\n" % e)
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

# **get_payment**
> PaymentResponse get_payment(payment_id)

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
        api_response = api_instance.get_payment(payment_id)
        print("The response of PaymentsApi->get_payment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->get_payment: %s\n" % e)
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

# **list_document_payments**
> PaymentsListResponse list_document_payments(document_id, limit=limit, cursor=cursor)

List Document Payments

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
    document_id = 'document_id_example' # str | 
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Document Payments
        api_response = api_instance.list_document_payments(document_id, limit=limit, cursor=cursor)
        print("The response of PaymentsApi->list_document_payments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->list_document_payments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
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

# **update_payment**
> PaymentResponse update_payment(payment_id, payment_patch_request)

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
        api_response = api_instance.update_payment(payment_id, payment_patch_request)
        print("The response of PaymentsApi->update_payment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentsApi->update_payment: %s\n" % e)
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

