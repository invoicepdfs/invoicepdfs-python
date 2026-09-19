# invoicepdfs.BrandingProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_branding_profile**](BrandingProfilesApi.md#create_branding_profile) | **POST** /api/v1/branding-profiles | Create Branding Profile
[**delete_branding_logo**](BrandingProfilesApi.md#delete_branding_logo) | **DELETE** /api/v1/branding-profiles/{profile_id}/logo | Delete Branding Logo
[**delete_branding_profile**](BrandingProfilesApi.md#delete_branding_profile) | **DELETE** /api/v1/branding-profiles/{profile_id} | Delete Branding Profile
[**get_branding_profile**](BrandingProfilesApi.md#get_branding_profile) | **GET** /api/v1/branding-profiles/{profile_id} | Get Branding Profile
[**list_branding_profiles**](BrandingProfilesApi.md#list_branding_profiles) | **GET** /api/v1/branding-profiles | List Branding Profiles
[**set_default_branding_profile**](BrandingProfilesApi.md#set_default_branding_profile) | **POST** /api/v1/branding-profiles/{profile_id}/default | Set Default Branding Profile
[**update_branding_profile**](BrandingProfilesApi.md#update_branding_profile) | **PATCH** /api/v1/branding-profiles/{profile_id} | Update Branding Profile
[**upload_branding_logo**](BrandingProfilesApi.md#upload_branding_logo) | **POST** /api/v1/branding-profiles/{profile_id}/logo | Upload Branding Logo


# **create_branding_profile**
> BrandingProfileResponse create_branding_profile(branding_profile_create_request)

Create Branding Profile

Create a look: colours, logo, fonts and footer.  Applies on top of whichever template a render names, so one template can serve several brands. Mark one as the default and documents that name no profile will use it.

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
        # Create Branding Profile
        api_response = api_instance.create_branding_profile(branding_profile_create_request)
        print("The response of BrandingProfilesApi->create_branding_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->create_branding_profile: %s\n" % e)
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

# **delete_branding_logo**
> SimpleBoolResponse delete_branding_logo(profile_id)

Delete Branding Logo

Remove this profile's logo, leaving its colours and text intact.

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
        # Delete Branding Logo
        api_response = api_instance.delete_branding_logo(profile_id)
        print("The response of BrandingProfilesApi->delete_branding_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->delete_branding_logo: %s\n" % e)
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

# **delete_branding_profile**
> SimpleBoolResponse delete_branding_profile(profile_id)

Delete Branding Profile

Remove a branding profile.  Deleting the default is allowed: the oldest remaining profile becomes the default in its place, so documents that name no profile keep rendering.

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
        # Delete Branding Profile
        api_response = api_instance.delete_branding_profile(profile_id)
        print("The response of BrandingProfilesApi->delete_branding_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->delete_branding_profile: %s\n" % e)
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

# **get_branding_profile**
> BrandingProfileResponse get_branding_profile(profile_id)

Get Branding Profile

One branding profile.

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
        # Get Branding Profile
        api_response = api_instance.get_branding_profile(profile_id)
        print("The response of BrandingProfilesApi->get_branding_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->get_branding_profile: %s\n" % e)
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

# **list_branding_profiles**
> BrandingProfilesListResponse list_branding_profiles()

List Branding Profiles

The looks a document can be rendered in, newest first.  Colours, logo, fonts and footer text — how a document appears. Who it is issued by is a business profile, which is a different thing.

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
        # List Branding Profiles
        api_response = api_instance.list_branding_profiles()
        print("The response of BrandingProfilesApi->list_branding_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->list_branding_profiles: %s\n" % e)
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

# **set_default_branding_profile**
> BrandingProfileResponse set_default_branding_profile(profile_id)

Set Default Branding Profile

Make this the profile used when a document names none.  Exactly one profile is the default; setting a new one clears the previous.

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
        # Set Default Branding Profile
        api_response = api_instance.set_default_branding_profile(profile_id)
        print("The response of BrandingProfilesApi->set_default_branding_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->set_default_branding_profile: %s\n" % e)
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

# **update_branding_profile**
> BrandingProfileResponse update_branding_profile(profile_id, branding_profile_patch_request)

Update Branding Profile

Change a branding profile.  Only the fields you send are changed. `hide_invoicepdfs_branding` is stored on any plan but only honoured on a plan that includes it — it is applied when a document renders, not validated here, so setting it on a plan without it is accepted and has no effect.

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
        # Update Branding Profile
        api_response = api_instance.update_branding_profile(profile_id, branding_profile_patch_request)
        print("The response of BrandingProfilesApi->update_branding_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->update_branding_profile: %s\n" % e)
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

# **upload_branding_logo**
> BrandingProfileResponse upload_branding_logo(profile_id, file)

Upload Branding Logo

Attach a logo image to this branding profile.  Replaces whatever logo the profile carried. The image is embedded when a document renders, so a later change applies to future renders and leaves PDFs already produced as they were.

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
        # Upload Branding Logo
        api_response = api_instance.upload_branding_logo(profile_id, file)
        print("The response of BrandingProfilesApi->upload_branding_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandingProfilesApi->upload_branding_logo: %s\n" % e)
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

