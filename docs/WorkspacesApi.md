# invoicepdfs.WorkspacesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_member_api_v1_workspaces_workspace_id_members_post**](WorkspacesApi.md#create_member_api_v1_workspaces_workspace_id_members_post) | **POST** /api/v1/workspaces/{workspace_id}/members | Create Member
[**create_workspace_api_v1_workspaces_post**](WorkspacesApi.md#create_workspace_api_v1_workspaces_post) | **POST** /api/v1/workspaces | Create Workspace
[**delete_member_api_v1_workspaces_workspace_id_members_member_id_delete**](WorkspacesApi.md#delete_member_api_v1_workspaces_workspace_id_members_member_id_delete) | **DELETE** /api/v1/workspaces/{workspace_id}/members/{member_id} | Delete Member
[**delete_workspace_api_v1_workspaces_workspace_id_delete**](WorkspacesApi.md#delete_workspace_api_v1_workspaces_workspace_id_delete) | **DELETE** /api/v1/workspaces/{workspace_id} | Delete Workspace
[**get_workspace_api_v1_workspaces_workspace_id_get**](WorkspacesApi.md#get_workspace_api_v1_workspaces_workspace_id_get) | **GET** /api/v1/workspaces/{workspace_id} | Get Workspace
[**list_members_api_v1_workspaces_workspace_id_members_get**](WorkspacesApi.md#list_members_api_v1_workspaces_workspace_id_members_get) | **GET** /api/v1/workspaces/{workspace_id}/members | List Members
[**list_workspaces_api_v1_workspaces_get**](WorkspacesApi.md#list_workspaces_api_v1_workspaces_get) | **GET** /api/v1/workspaces | List Workspaces
[**patch_member_api_v1_workspaces_workspace_id_members_member_id_patch**](WorkspacesApi.md#patch_member_api_v1_workspaces_workspace_id_members_member_id_patch) | **PATCH** /api/v1/workspaces/{workspace_id}/members/{member_id} | Patch Member
[**patch_workspace_api_v1_workspaces_workspace_id_patch**](WorkspacesApi.md#patch_workspace_api_v1_workspaces_workspace_id_patch) | **PATCH** /api/v1/workspaces/{workspace_id} | Patch Workspace


# **create_member_api_v1_workspaces_workspace_id_members_post**
> WorkspaceMembersListResponse create_member_api_v1_workspaces_workspace_id_members_post(workspace_id, workspace_member_create_request, idempotency_key=idempotency_key)

Create Member

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_member_create_request import WorkspaceMemberCreateRequest
from invoicepdfs.models.workspace_members_list_response import WorkspaceMembersListResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    workspace_member_create_request = invoicepdfs.WorkspaceMemberCreateRequest() # WorkspaceMemberCreateRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Member
        api_response = api_instance.create_member_api_v1_workspaces_workspace_id_members_post(workspace_id, workspace_member_create_request, idempotency_key=idempotency_key)
        print("The response of WorkspacesApi->create_member_api_v1_workspaces_workspace_id_members_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->create_member_api_v1_workspaces_workspace_id_members_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **workspace_member_create_request** | [**WorkspaceMemberCreateRequest**](WorkspaceMemberCreateRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**WorkspaceMembersListResponse**](WorkspaceMembersListResponse.md)

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

# **create_workspace_api_v1_workspaces_post**
> WorkspaceResponse create_workspace_api_v1_workspaces_post(workspace_create_request, idempotency_key=idempotency_key)

Create Workspace

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_create_request import WorkspaceCreateRequest
from invoicepdfs.models.workspace_response import WorkspaceResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_create_request = invoicepdfs.WorkspaceCreateRequest() # WorkspaceCreateRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Create Workspace
        api_response = api_instance.create_workspace_api_v1_workspaces_post(workspace_create_request, idempotency_key=idempotency_key)
        print("The response of WorkspacesApi->create_workspace_api_v1_workspaces_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->create_workspace_api_v1_workspaces_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_create_request** | [**WorkspaceCreateRequest**](WorkspaceCreateRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

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

# **delete_member_api_v1_workspaces_workspace_id_members_member_id_delete**
> SimpleBoolResponse delete_member_api_v1_workspaces_workspace_id_members_member_id_delete(workspace_id, member_id)

Delete Member

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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    member_id = 'member_id_example' # str | 

    try:
        # Delete Member
        api_response = api_instance.delete_member_api_v1_workspaces_workspace_id_members_member_id_delete(workspace_id, member_id)
        print("The response of WorkspacesApi->delete_member_api_v1_workspaces_workspace_id_members_member_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->delete_member_api_v1_workspaces_workspace_id_members_member_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **member_id** | **str**|  | 

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

# **delete_workspace_api_v1_workspaces_workspace_id_delete**
> SimpleBoolResponse delete_workspace_api_v1_workspaces_workspace_id_delete(workspace_id)

Delete Workspace

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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 

    try:
        # Delete Workspace
        api_response = api_instance.delete_workspace_api_v1_workspaces_workspace_id_delete(workspace_id)
        print("The response of WorkspacesApi->delete_workspace_api_v1_workspaces_workspace_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->delete_workspace_api_v1_workspaces_workspace_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 

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

# **get_workspace_api_v1_workspaces_workspace_id_get**
> WorkspaceResponse get_workspace_api_v1_workspaces_workspace_id_get(workspace_id)

Get Workspace

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_response import WorkspaceResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 

    try:
        # Get Workspace
        api_response = api_instance.get_workspace_api_v1_workspaces_workspace_id_get(workspace_id)
        print("The response of WorkspacesApi->get_workspace_api_v1_workspaces_workspace_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->get_workspace_api_v1_workspaces_workspace_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 

### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

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

# **list_members_api_v1_workspaces_workspace_id_members_get**
> WorkspaceMembersListResponse list_members_api_v1_workspaces_workspace_id_members_get(workspace_id)

List Members

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_members_list_response import WorkspaceMembersListResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 

    try:
        # List Members
        api_response = api_instance.list_members_api_v1_workspaces_workspace_id_members_get(workspace_id)
        print("The response of WorkspacesApi->list_members_api_v1_workspaces_workspace_id_members_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->list_members_api_v1_workspaces_workspace_id_members_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 

### Return type

[**WorkspaceMembersListResponse**](WorkspaceMembersListResponse.md)

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

# **list_workspaces_api_v1_workspaces_get**
> WorkspacesListResponse list_workspaces_api_v1_workspaces_get(limit=limit, cursor=cursor)

List Workspaces

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspaces_list_response import WorkspacesListResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Workspaces
        api_response = api_instance.list_workspaces_api_v1_workspaces_get(limit=limit, cursor=cursor)
        print("The response of WorkspacesApi->list_workspaces_api_v1_workspaces_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->list_workspaces_api_v1_workspaces_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**WorkspacesListResponse**](WorkspacesListResponse.md)

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

# **patch_member_api_v1_workspaces_workspace_id_members_member_id_patch**
> WorkspaceMemberOut patch_member_api_v1_workspaces_workspace_id_members_member_id_patch(workspace_id, member_id, workspace_member_patch_request)

Patch Member

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_member_out import WorkspaceMemberOut
from invoicepdfs.models.workspace_member_patch_request import WorkspaceMemberPatchRequest
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    member_id = 'member_id_example' # str | 
    workspace_member_patch_request = invoicepdfs.WorkspaceMemberPatchRequest() # WorkspaceMemberPatchRequest | 

    try:
        # Patch Member
        api_response = api_instance.patch_member_api_v1_workspaces_workspace_id_members_member_id_patch(workspace_id, member_id, workspace_member_patch_request)
        print("The response of WorkspacesApi->patch_member_api_v1_workspaces_workspace_id_members_member_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->patch_member_api_v1_workspaces_workspace_id_members_member_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **member_id** | **str**|  | 
 **workspace_member_patch_request** | [**WorkspaceMemberPatchRequest**](WorkspaceMemberPatchRequest.md)|  | 

### Return type

[**WorkspaceMemberOut**](WorkspaceMemberOut.md)

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

# **patch_workspace_api_v1_workspaces_workspace_id_patch**
> WorkspaceResponse patch_workspace_api_v1_workspaces_workspace_id_patch(workspace_id, workspace_patch_request, idempotency_key=idempotency_key)

Patch Workspace

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.workspace_patch_request import WorkspacePatchRequest
from invoicepdfs.models.workspace_response import WorkspaceResponse
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
    api_instance = invoicepdfs.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    workspace_patch_request = invoicepdfs.WorkspacePatchRequest() # WorkspacePatchRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Patch Workspace
        api_response = api_instance.patch_workspace_api_v1_workspaces_workspace_id_patch(workspace_id, workspace_patch_request, idempotency_key=idempotency_key)
        print("The response of WorkspacesApi->patch_workspace_api_v1_workspaces_workspace_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->patch_workspace_api_v1_workspaces_workspace_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **workspace_patch_request** | [**WorkspacePatchRequest**](WorkspacePatchRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

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

