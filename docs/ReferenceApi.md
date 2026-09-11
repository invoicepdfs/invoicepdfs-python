# invoicepdfs.ReferenceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_countries**](ReferenceApi.md#list_countries) | **GET** /api/v1/reference/countries | List Countries
[**list_currencies**](ReferenceApi.md#list_currencies) | **GET** /api/v1/reference/currencies | List Currencies
[**list_document_types**](ReferenceApi.md#list_document_types) | **GET** /api/v1/reference/document-types | List Document Types
[**list_locales**](ReferenceApi.md#list_locales) | **GET** /api/v1/reference/locales | List Locales
[**list_page_sizes**](ReferenceApi.md#list_page_sizes) | **GET** /api/v1/reference/page-sizes | List Page Sizes
[**list_tax_categories**](ReferenceApi.md#list_tax_categories) | **GET** /api/v1/reference/tax-categories | List Tax Categories
[**list_tax_schemes**](ReferenceApi.md#list_tax_schemes) | **GET** /api/v1/reference/tax-schemes | List Tax Schemes
[**list_timezones**](ReferenceApi.md#list_timezones) | **GET** /api/v1/reference/timezones | List Timezones
[**list_unit_codes**](ReferenceApi.md#list_unit_codes) | **GET** /api/v1/reference/unit-codes | List Unit Codes


# **list_countries**
> CountriesListResponse list_countries()

List Countries

### Example


```python
import invoicepdfs
from invoicepdfs.models.countries_list_response import CountriesListResponse
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

[**CountriesListResponse**](CountriesListResponse.md)

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
> CurrenciesListResponse list_currencies()

List Currencies

### Example


```python
import invoicepdfs
from invoicepdfs.models.currencies_list_response import CurrenciesListResponse
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

[**CurrenciesListResponse**](CurrenciesListResponse.md)

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
> DocumentTypesListResponse list_document_types()

List Document Types

List every supported document type with the metadata a client needs to build a type-aware create form: the number prefix, whether it is payable / takes a source document / supports a reason, which line-item shape it uses (``standard`` = priced, ``shipped`` = quantities only), and the lifecycle actions available to it.

### Example


```python
import invoicepdfs
from invoicepdfs.models.document_types_list_response import DocumentTypesListResponse
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

[**DocumentTypesListResponse**](DocumentTypesListResponse.md)

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
> LocalesListResponse list_locales()

List Locales

### Example


```python
import invoicepdfs
from invoicepdfs.models.locales_list_response import LocalesListResponse
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

[**LocalesListResponse**](LocalesListResponse.md)

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
> PageSizesListResponse list_page_sizes()

List Page Sizes

### Example


```python
import invoicepdfs
from invoicepdfs.models.page_sizes_list_response import PageSizesListResponse
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

[**PageSizesListResponse**](PageSizesListResponse.md)

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

# **list_tax_categories**
> CodeListResponse list_tax_categories()

List Tax Categories

UNCL5305, in full — the VAT treatment of a line, which its rate does not say.  Two lines at 0% may be zero-rated, exempt, reverse-charge or outside scope, and EN 16931 puts them in separate VAT breakdown groups with different mandatory fields. Exhaustive: a category outside this list is wrong.

### Example


```python
import invoicepdfs
from invoicepdfs.models.code_list_response import CodeListResponse
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
        # List Tax Categories
        api_response = api_instance.list_tax_categories()
        print("The response of ReferenceApi->list_tax_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_tax_categories: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CodeListResponse**](CodeListResponse.md)

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

# **list_tax_schemes**
> CodeListResponse list_tax_schemes()

List Tax Schemes

UNCL5153 — which tax regime a document is issued under, one per document.  `VAT` is the only member an e-invoice can carry; the others exist so a caller can state that their tax is *not* VAT and be told so, rather than have VAT assumed on their behalf. There is no default: a PDF does not need a scheme, and guessing one puts a claim in a document a tax authority reads that the caller never made.

### Example


```python
import invoicepdfs
from invoicepdfs.models.code_list_response import CodeListResponse
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
        # List Tax Schemes
        api_response = api_instance.list_tax_schemes()
        print("The response of ReferenceApi->list_tax_schemes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_tax_schemes: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CodeListResponse**](CodeListResponse.md)

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
> TimezonesListResponse list_timezones()

List Timezones

### Example


```python
import invoicepdfs
from invoicepdfs.models.timezones_list_response import TimezonesListResponse
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

[**TimezonesListResponse**](TimezonesListResponse.md)

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

# **list_unit_codes**
> CodeListResponse list_unit_codes()

List Unit Codes

UN/ECE Recommendation 20 — the unit a line item is measured in.  A **shortlist**: twenty-one of hundreds, ordered by how often an invoice needs them. `exhaustive` is false, and it means it — `unit_code` accepts any value, nothing validates against this list, and an uncommon code is still correct. Offered because the field takes a code rather than the printed label: mapping \"hrs\" to HUR is an inference that is right until it silently is not, and the audience for the result is a tax authority.

### Example


```python
import invoicepdfs
from invoicepdfs.models.code_list_response import CodeListResponse
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
        # List Unit Codes
        api_response = api_instance.list_unit_codes()
        print("The response of ReferenceApi->list_unit_codes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferenceApi->list_unit_codes: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CodeListResponse**](CodeListResponse.md)

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

