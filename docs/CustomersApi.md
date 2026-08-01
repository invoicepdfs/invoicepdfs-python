# invoicepdfs.CustomersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_customer_api_v1_customers_post**](CustomersApi.md#create_customer_api_v1_customers_post) | **POST** /api/v1/customers | Create Customer
[**delete_customer_api_v1_customers_customer_id_delete**](CustomersApi.md#delete_customer_api_v1_customers_customer_id_delete) | **DELETE** /api/v1/customers/{customer_id} | Delete Customer
[**get_customer_api_v1_customers_customer_id_get**](CustomersApi.md#get_customer_api_v1_customers_customer_id_get) | **GET** /api/v1/customers/{customer_id} | Get Customer
[**list_customers_api_v1_customers_get**](CustomersApi.md#list_customers_api_v1_customers_get) | **GET** /api/v1/customers | List Customers
[**patch_customer_api_v1_customers_customer_id_patch**](CustomersApi.md#patch_customer_api_v1_customers_customer_id_patch) | **PATCH** /api/v1/customers/{customer_id} | Patch Customer


# **create_customer_api_v1_customers_post**
> CustomerResponse create_customer_api_v1_customers_post(customer_create, idempotency_key=idempotency_key)

Create Customer

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.customer_create import CustomerCreate
from invoicepdfs.models.customer_response import CustomerResponse
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
    api_instance = invoicepdfs.CustomersApi(api_client)
    customer_create = invoicepdfs.CustomerCreate() # CustomerCreate | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Customer
        api_response = api_instance.create_customer_api_v1_customers_post(customer_create, idempotency_key=idempotency_key)
        print("The response of CustomersApi->create_customer_api_v1_customers_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->create_customer_api_v1_customers_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_create** | [**CustomerCreate**](CustomerCreate.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**CustomerResponse**](CustomerResponse.md)

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

# **delete_customer_api_v1_customers_customer_id_delete**
> SimpleBoolResponse delete_customer_api_v1_customers_customer_id_delete(customer_id)

Delete Customer

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
    api_instance = invoicepdfs.CustomersApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        # Delete Customer
        api_response = api_instance.delete_customer_api_v1_customers_customer_id_delete(customer_id)
        print("The response of CustomersApi->delete_customer_api_v1_customers_customer_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->delete_customer_api_v1_customers_customer_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

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

# **get_customer_api_v1_customers_customer_id_get**
> CustomerResponse get_customer_api_v1_customers_customer_id_get(customer_id)

Get Customer

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.customer_response import CustomerResponse
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
    api_instance = invoicepdfs.CustomersApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        # Get Customer
        api_response = api_instance.get_customer_api_v1_customers_customer_id_get(customer_id)
        print("The response of CustomersApi->get_customer_api_v1_customers_customer_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->get_customer_api_v1_customers_customer_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

### Return type

[**CustomerResponse**](CustomerResponse.md)

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

# **list_customers_api_v1_customers_get**
> CustomersListResponse list_customers_api_v1_customers_get(limit=limit, cursor=cursor)

List Customers

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.customers_list_response import CustomersListResponse
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
    api_instance = invoicepdfs.CustomersApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Customers
        api_response = api_instance.list_customers_api_v1_customers_get(limit=limit, cursor=cursor)
        print("The response of CustomersApi->list_customers_api_v1_customers_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->list_customers_api_v1_customers_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**CustomersListResponse**](CustomersListResponse.md)

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

# **patch_customer_api_v1_customers_customer_id_patch**
> CustomerResponse patch_customer_api_v1_customers_customer_id_patch(customer_id, customer_patch, idempotency_key=idempotency_key)

Patch Customer

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.customer_patch import CustomerPatch
from invoicepdfs.models.customer_response import CustomerResponse
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
    api_instance = invoicepdfs.CustomersApi(api_client)
    customer_id = 'customer_id_example' # str | 
    customer_patch = invoicepdfs.CustomerPatch() # CustomerPatch | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Patch Customer
        api_response = api_instance.patch_customer_api_v1_customers_customer_id_patch(customer_id, customer_patch, idempotency_key=idempotency_key)
        print("The response of CustomersApi->patch_customer_api_v1_customers_customer_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->patch_customer_api_v1_customers_customer_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 
 **customer_patch** | [**CustomerPatch**](CustomerPatch.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**CustomerResponse**](CustomerResponse.md)

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

