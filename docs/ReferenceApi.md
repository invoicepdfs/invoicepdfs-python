# invoicepdfs.ReferenceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_countries_api_v1_reference_countries_get**](ReferenceApi.md#list_countries_api_v1_reference_countries_get) | **GET** /api/v1/reference/countries | List Countries
[**list_currencies_api_v1_reference_currencies_get**](ReferenceApi.md#list_currencies_api_v1_reference_currencies_get) | **GET** /api/v1/reference/currencies | List Currencies
[**list_document_types_api_v1_reference_document_types_get**](ReferenceApi.md#list_document_types_api_v1_reference_document_types_get) | **GET** /api/v1/reference/document-types | List Document Types
[**list_locales_api_v1_reference_locales_get**](ReferenceApi.md#list_locales_api_v1_reference_locales_get) | **GET** /api/v1/reference/locales | List Locales
[**list_page_sizes_api_v1_reference_page_sizes_get**](ReferenceApi.md#list_page_sizes_api_v1_reference_page_sizes_get) | **GET** /api/v1/reference/page-sizes | List Page Sizes
[**list_timezones_api_v1_reference_timezones_get**](ReferenceApi.md#list_timezones_api_v1_reference_timezones_get) | **GET** /api/v1/reference/timezones | List Timezones


# **list_countries_api_v1_reference_countries_get**
> Dict[str, object] list_countries_api_v1_reference_countries_get()

List Countries

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Countries
        api_response = api_instance.list_countries_api_v1_reference_countries_get()
        print("The response of ReferenceApi->list_countries_api_v1_reference_countries_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_countries_api_v1_reference_countries_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_currencies_api_v1_reference_currencies_get**
> Dict[str, object] list_currencies_api_v1_reference_currencies_get()

List Currencies

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Currencies
        api_response = api_instance.list_currencies_api_v1_reference_currencies_get()
        print("The response of ReferenceApi->list_currencies_api_v1_reference_currencies_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_currencies_api_v1_reference_currencies_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_document_types_api_v1_reference_document_types_get**
> Dict[str, object] list_document_types_api_v1_reference_document_types_get()

List Document Types

List every supported document type with the metadata a client needs to build a type-aware create form: the number prefix, whether it is payable / takes a source document / supports a reason, which line-item shape it uses (``standard`` = priced, ``shipped`` = quantities only), and the lifecycle actions available to it.

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Document Types
        api_response = api_instance.list_document_types_api_v1_reference_document_types_get()
        print("The response of ReferenceApi->list_document_types_api_v1_reference_document_types_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_document_types_api_v1_reference_document_types_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_locales_api_v1_reference_locales_get**
> Dict[str, object] list_locales_api_v1_reference_locales_get()

List Locales

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Locales
        api_response = api_instance.list_locales_api_v1_reference_locales_get()
        print("The response of ReferenceApi->list_locales_api_v1_reference_locales_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_locales_api_v1_reference_locales_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_page_sizes_api_v1_reference_page_sizes_get**
> Dict[str, object] list_page_sizes_api_v1_reference_page_sizes_get()

List Page Sizes

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Page Sizes
        api_response = api_instance.list_page_sizes_api_v1_reference_page_sizes_get()
        print("The response of ReferenceApi->list_page_sizes_api_v1_reference_page_sizes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_page_sizes_api_v1_reference_page_sizes_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_timezones_api_v1_reference_timezones_get**
> Dict[str, object] list_timezones_api_v1_reference_timezones_get()

List Timezones

### Example


```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ReferenceApi(api_client)

    try:
        # List Timezones
        api_response = api_instance.list_timezones_api_v1_reference_timezones_get()
        print("The response of ReferenceApi->list_timezones_api_v1_reference_timezones_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_timezones_api_v1_reference_timezones_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**Dict[str, object]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

