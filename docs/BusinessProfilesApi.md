# invoicepdfs.BusinessProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_business_profile**](BusinessProfilesApi.md#create_business_profile) | **POST** /api/v1/business-profiles | Create Business Profile
[**delete_business_profile**](BusinessProfilesApi.md#delete_business_profile) | **DELETE** /api/v1/business-profiles/{business_profile_id} | Delete Business Profile
[**get_business_profile**](BusinessProfilesApi.md#get_business_profile) | **GET** /api/v1/business-profiles/{business_profile_id} | Get Business Profile
[**list_business_profiles**](BusinessProfilesApi.md#list_business_profiles) | **GET** /api/v1/business-profiles | List Business Profiles
[**update_business_profile**](BusinessProfilesApi.md#update_business_profile) | **PATCH** /api/v1/business-profiles/{business_profile_id} | Update Business Profile


# **create_business_profile**
> BusinessProfileResponse create_business_profile(business_profile_create, idempotency_key=idempotency_key)

Create Business Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.business_profile_create import BusinessProfileCreate
from invoicepdfs.models.business_profile_response import BusinessProfileResponse
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
    api_instance = invoicepdfs.BusinessProfilesApi(api_client)
    business_profile_create = invoicepdfs.BusinessProfileCreate() # BusinessProfileCreate | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Business Profile
        api_response = api_instance.create_business_profile(business_profile_create, idempotency_key=idempotency_key)
        print("The response of BusinessProfilesApi->create_business_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BusinessProfilesApi->create_business_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **business_profile_create** | [**BusinessProfileCreate**](BusinessProfileCreate.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

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

# **delete_business_profile**
> SimpleBoolResponse delete_business_profile(business_profile_id)

Delete Business Profile

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
    api_instance = invoicepdfs.BusinessProfilesApi(api_client)
    business_profile_id = 'business_profile_id_example' # str | 

    try:
        # Delete Business Profile
        api_response = api_instance.delete_business_profile(business_profile_id)
        print("The response of BusinessProfilesApi->delete_business_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BusinessProfilesApi->delete_business_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **business_profile_id** | **str**|  | 

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

# **get_business_profile**
> BusinessProfileResponse get_business_profile(business_profile_id)

Get Business Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.business_profile_response import BusinessProfileResponse
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
    api_instance = invoicepdfs.BusinessProfilesApi(api_client)
    business_profile_id = 'business_profile_id_example' # str | 

    try:
        # Get Business Profile
        api_response = api_instance.get_business_profile(business_profile_id)
        print("The response of BusinessProfilesApi->get_business_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BusinessProfilesApi->get_business_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **business_profile_id** | **str**|  | 

### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

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

# **list_business_profiles**
> BusinessProfilesListResponse list_business_profiles(limit=limit, cursor=cursor)

List Business Profiles

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.business_profiles_list_response import BusinessProfilesListResponse
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
    api_instance = invoicepdfs.BusinessProfilesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Business Profiles
        api_response = api_instance.list_business_profiles(limit=limit, cursor=cursor)
        print("The response of BusinessProfilesApi->list_business_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BusinessProfilesApi->list_business_profiles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**BusinessProfilesListResponse**](BusinessProfilesListResponse.md)

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

# **update_business_profile**
> BusinessProfileResponse update_business_profile(business_profile_id, business_profile_patch, idempotency_key=idempotency_key)

Update Business Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.business_profile_patch import BusinessProfilePatch
from invoicepdfs.models.business_profile_response import BusinessProfileResponse
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
    api_instance = invoicepdfs.BusinessProfilesApi(api_client)
    business_profile_id = 'business_profile_id_example' # str | 
    business_profile_patch = invoicepdfs.BusinessProfilePatch() # BusinessProfilePatch | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Update Business Profile
        api_response = api_instance.update_business_profile(business_profile_id, business_profile_patch, idempotency_key=idempotency_key)
        print("The response of BusinessProfilesApi->update_business_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BusinessProfilesApi->update_business_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **business_profile_id** | **str**|  | 
 **business_profile_patch** | [**BusinessProfilePatch**](BusinessProfilePatch.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

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

