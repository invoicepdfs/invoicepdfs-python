# invoicepdfs.BrandingProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_profile_api_v1_branding_profiles_post**](BrandingProfilesApi.md#create_profile_api_v1_branding_profiles_post) | **POST** /api/v1/branding-profiles | Create Profile
[**delete_logo_api_v1_branding_profiles_profile_id_logo_delete**](BrandingProfilesApi.md#delete_logo_api_v1_branding_profiles_profile_id_logo_delete) | **DELETE** /api/v1/branding-profiles/{profile_id}/logo | Delete Logo
[**delete_profile_api_v1_branding_profiles_profile_id_delete**](BrandingProfilesApi.md#delete_profile_api_v1_branding_profiles_profile_id_delete) | **DELETE** /api/v1/branding-profiles/{profile_id} | Delete Profile
[**get_profile_api_v1_branding_profiles_profile_id_get**](BrandingProfilesApi.md#get_profile_api_v1_branding_profiles_profile_id_get) | **GET** /api/v1/branding-profiles/{profile_id} | Get Profile
[**list_profiles_api_v1_branding_profiles_get**](BrandingProfilesApi.md#list_profiles_api_v1_branding_profiles_get) | **GET** /api/v1/branding-profiles | List Profiles
[**set_default_api_v1_branding_profiles_profile_id_default_post**](BrandingProfilesApi.md#set_default_api_v1_branding_profiles_profile_id_default_post) | **POST** /api/v1/branding-profiles/{profile_id}/default | Set Default
[**update_profile_api_v1_branding_profiles_profile_id_patch**](BrandingProfilesApi.md#update_profile_api_v1_branding_profiles_profile_id_patch) | **PATCH** /api/v1/branding-profiles/{profile_id} | Update Profile
[**upload_logo_api_v1_branding_profiles_profile_id_logo_post**](BrandingProfilesApi.md#upload_logo_api_v1_branding_profiles_profile_id_logo_post) | **POST** /api/v1/branding-profiles/{profile_id}/logo | Upload Logo


# **create_profile_api_v1_branding_profiles_post**
> BrandingProfileResponse create_profile_api_v1_branding_profiles_post(branding_profile_create_request)

Create Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profile_create_request import BrandingProfileCreateRequest
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    branding_profile_create_request = invoicepdfs.BrandingProfileCreateRequest() # BrandingProfileCreateRequest | 

    try:
        # Create Profile
        api_response = api_instance.create_profile_api_v1_branding_profiles_post(branding_profile_create_request)
        print("The response of BrandingProfilesApi->create_profile_api_v1_branding_profiles_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->create_profile_api_v1_branding_profiles_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **branding_profile_create_request** | [**BrandingProfileCreateRequest**](BrandingProfileCreateRequest.md)|  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

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

# **delete_logo_api_v1_branding_profiles_profile_id_logo_delete**
> SimpleBoolResponse delete_logo_api_v1_branding_profiles_profile_id_logo_delete(profile_id)

Delete Logo

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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Delete Logo
        api_response = api_instance.delete_logo_api_v1_branding_profiles_profile_id_logo_delete(profile_id)
        print("The response of BrandingProfilesApi->delete_logo_api_v1_branding_profiles_profile_id_logo_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->delete_logo_api_v1_branding_profiles_profile_id_logo_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

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

# **delete_profile_api_v1_branding_profiles_profile_id_delete**
> SimpleBoolResponse delete_profile_api_v1_branding_profiles_profile_id_delete(profile_id)

Delete Profile

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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Delete Profile
        api_response = api_instance.delete_profile_api_v1_branding_profiles_profile_id_delete(profile_id)
        print("The response of BrandingProfilesApi->delete_profile_api_v1_branding_profiles_profile_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->delete_profile_api_v1_branding_profiles_profile_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

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

# **get_profile_api_v1_branding_profiles_profile_id_get**
> BrandingProfileResponse get_profile_api_v1_branding_profiles_profile_id_get(profile_id)

Get Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Get Profile
        api_response = api_instance.get_profile_api_v1_branding_profiles_profile_id_get(profile_id)
        print("The response of BrandingProfilesApi->get_profile_api_v1_branding_profiles_profile_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->get_profile_api_v1_branding_profiles_profile_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

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

# **list_profiles_api_v1_branding_profiles_get**
> BrandingProfilesListResponse list_profiles_api_v1_branding_profiles_get()

List Profiles

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profiles_list_response import BrandingProfilesListResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)

    try:
        # List Profiles
        api_response = api_instance.list_profiles_api_v1_branding_profiles_get()
        print("The response of BrandingProfilesApi->list_profiles_api_v1_branding_profiles_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->list_profiles_api_v1_branding_profiles_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**BrandingProfilesListResponse**](BrandingProfilesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_default_api_v1_branding_profiles_profile_id_default_post**
> BrandingProfileResponse set_default_api_v1_branding_profiles_profile_id_default_post(profile_id)

Set Default

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Set Default
        api_response = api_instance.set_default_api_v1_branding_profiles_profile_id_default_post(profile_id)
        print("The response of BrandingProfilesApi->set_default_api_v1_branding_profiles_profile_id_default_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->set_default_api_v1_branding_profiles_profile_id_default_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

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

# **update_profile_api_v1_branding_profiles_profile_id_patch**
> BrandingProfileResponse update_profile_api_v1_branding_profiles_profile_id_patch(profile_id, branding_profile_patch_request)

Update Profile

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profile_patch_request import BrandingProfilePatchRequest
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 
    branding_profile_patch_request = invoicepdfs.BrandingProfilePatchRequest() # BrandingProfilePatchRequest | 

    try:
        # Update Profile
        api_response = api_instance.update_profile_api_v1_branding_profiles_profile_id_patch(profile_id, branding_profile_patch_request)
        print("The response of BrandingProfilesApi->update_profile_api_v1_branding_profiles_profile_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->update_profile_api_v1_branding_profiles_profile_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **branding_profile_patch_request** | [**BrandingProfilePatchRequest**](BrandingProfilePatchRequest.md)|  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

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

# **upload_logo_api_v1_branding_profiles_profile_id_logo_post**
> BrandingProfileResponse upload_logo_api_v1_branding_profiles_profile_id_logo_post(profile_id, file)

Upload Logo

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse
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
    api_instance = invoicepdfs.BrandingProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 
    file = None # bytearray | 

    try:
        # Upload Logo
        api_response = api_instance.upload_logo_api_v1_branding_profiles_profile_id_logo_post(profile_id, file)
        print("The response of BrandingProfilesApi->upload_logo_api_v1_branding_profiles_profile_id_logo_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->upload_logo_api_v1_branding_profiles_profile_id_logo_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **file** | **bytearray**|  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

