# invoicepdfs.TaxRatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tax_rate**](TaxRatesApi.md#create_tax_rate) | **POST** /api/v1/tax-rates | Create Tax Rate
[**delete_tax_rate**](TaxRatesApi.md#delete_tax_rate) | **DELETE** /api/v1/tax-rates/{tax_rate_id} | Delete Tax Rate
[**get_tax_rate**](TaxRatesApi.md#get_tax_rate) | **GET** /api/v1/tax-rates/{tax_rate_id} | Get Tax Rate
[**list_tax_rates**](TaxRatesApi.md#list_tax_rates) | **GET** /api/v1/tax-rates | List Tax Rates
[**update_tax_rate**](TaxRatesApi.md#update_tax_rate) | **PATCH** /api/v1/tax-rates/{tax_rate_id} | Update Tax Rate


# **create_tax_rate**
> TaxRateResponse create_tax_rate(tax_rate_create_request)

Create Tax Rate

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.tax_rate_create_request import TaxRateCreateRequest
from invoicepdfs.models.tax_rate_response import TaxRateResponse
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
    api_instance = invoicepdfs.TaxRatesApi(api_client)
    tax_rate_create_request = invoicepdfs.TaxRateCreateRequest() # TaxRateCreateRequest | 

    try:
        # Create Tax Rate
        api_response = api_instance.create_tax_rate(tax_rate_create_request)
        print("The response of TaxRatesApi->create_tax_rate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaxRatesApi->create_tax_rate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tax_rate_create_request** | [**TaxRateCreateRequest**](TaxRateCreateRequest.md)|  | 

### Return type

[**TaxRateResponse**](TaxRateResponse.md)

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

# **delete_tax_rate**
> SimpleBoolResponse delete_tax_rate(tax_rate_id)

Delete Tax Rate

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
    api_instance = invoicepdfs.TaxRatesApi(api_client)
    tax_rate_id = 'tax_rate_id_example' # str | 

    try:
        # Delete Tax Rate
        api_response = api_instance.delete_tax_rate(tax_rate_id)
        print("The response of TaxRatesApi->delete_tax_rate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaxRatesApi->delete_tax_rate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tax_rate_id** | **str**|  | 

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

# **get_tax_rate**
> TaxRateResponse get_tax_rate(tax_rate_id)

Get Tax Rate

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.tax_rate_response import TaxRateResponse
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
    api_instance = invoicepdfs.TaxRatesApi(api_client)
    tax_rate_id = 'tax_rate_id_example' # str | 

    try:
        # Get Tax Rate
        api_response = api_instance.get_tax_rate(tax_rate_id)
        print("The response of TaxRatesApi->get_tax_rate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaxRatesApi->get_tax_rate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tax_rate_id** | **str**|  | 

### Return type

[**TaxRateResponse**](TaxRateResponse.md)

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

# **list_tax_rates**
> TaxRatesListResponse list_tax_rates(limit=limit, cursor=cursor)

List Tax Rates

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.tax_rates_list_response import TaxRatesListResponse
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
    api_instance = invoicepdfs.TaxRatesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Tax Rates
        api_response = api_instance.list_tax_rates(limit=limit, cursor=cursor)
        print("The response of TaxRatesApi->list_tax_rates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaxRatesApi->list_tax_rates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**TaxRatesListResponse**](TaxRatesListResponse.md)

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

# **update_tax_rate**
> TaxRateResponse update_tax_rate(tax_rate_id, tax_rate_patch_request)

Update Tax Rate

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.tax_rate_patch_request import TaxRatePatchRequest
from invoicepdfs.models.tax_rate_response import TaxRateResponse
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
    api_instance = invoicepdfs.TaxRatesApi(api_client)
    tax_rate_id = 'tax_rate_id_example' # str | 
    tax_rate_patch_request = invoicepdfs.TaxRatePatchRequest() # TaxRatePatchRequest | 

    try:
        # Update Tax Rate
        api_response = api_instance.update_tax_rate(tax_rate_id, tax_rate_patch_request)
        print("The response of TaxRatesApi->update_tax_rate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaxRatesApi->update_tax_rate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tax_rate_id** | **str**|  | 
 **tax_rate_patch_request** | [**TaxRatePatchRequest**](TaxRatePatchRequest.md)|  | 

### Return type

[**TaxRateResponse**](TaxRateResponse.md)

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

