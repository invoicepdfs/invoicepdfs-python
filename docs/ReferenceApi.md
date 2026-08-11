# invoicepdfs.ReferenceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_countries**](ReferenceApi.md#list_countries) | **GET** /api/v1/reference/countries | List Countries
[**list_currencies**](ReferenceApi.md#list_currencies) | **GET** /api/v1/reference/currencies | List Currencies
[**list_document_types**](ReferenceApi.md#list_document_types) | **GET** /api/v1/reference/document-types | List Document Types
[**list_locales**](ReferenceApi.md#list_locales) | **GET** /api/v1/reference/locales | List Locales
[**list_page_sizes**](ReferenceApi.md#list_page_sizes) | **GET** /api/v1/reference/page-sizes | List Page Sizes
[**list_timezones**](ReferenceApi.md#list_timezones) | **GET** /api/v1/reference/timezones | List Timezones


# **list_countries**
> Dict[str, object] list_countries()

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
        api_response = api_instance.list_countries()
        print("The response of ReferenceApi->list_countries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_countries: %s\n" % e)
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

# **list_currencies**
> Dict[str, object] list_currencies()

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
        api_response = api_instance.list_currencies()
        print("The response of ReferenceApi->list_currencies:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_currencies: %s\n" % e)
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

# **list_document_types**
> Dict[str, object] list_document_types()

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
        api_response = api_instance.list_document_types()
        print("The response of ReferenceApi->list_document_types:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_document_types: %s\n" % e)
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

# **list_locales**
> Dict[str, object] list_locales()

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
        api_response = api_instance.list_locales()
        print("The response of ReferenceApi->list_locales:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_locales: %s\n" % e)
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

# **list_page_sizes**
> Dict[str, object] list_page_sizes()

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
        api_response = api_instance.list_page_sizes()
        print("The response of ReferenceApi->list_page_sizes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_page_sizes: %s\n" % e)
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

# **list_timezones**
> Dict[str, object] list_timezones()

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
        api_response = api_instance.list_timezones()
        print("The response of ReferenceApi->list_timezones:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_timezones: %s\n" % e)
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

