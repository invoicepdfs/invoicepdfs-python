# invoicepdfs.TemplateVersionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_template_version_api_v1_templates_template_id_versions_post**](TemplateVersionsApi.md#create_template_version_api_v1_templates_template_id_versions_post) | **POST** /api/v1/templates/{template_id}/versions | Create Template Version
[**get_template_version_api_v1_templates_template_id_versions_version_get**](TemplateVersionsApi.md#get_template_version_api_v1_templates_template_id_versions_version_get) | **GET** /api/v1/templates/{template_id}/versions/{version} | Get Template Version
[**list_template_versions_api_v1_templates_template_id_versions_get**](TemplateVersionsApi.md#list_template_versions_api_v1_templates_template_id_versions_get) | **GET** /api/v1/templates/{template_id}/versions | List Template Versions


# **create_template_version_api_v1_templates_template_id_versions_post**
> TemplateVersionResponse create_template_version_api_v1_templates_template_id_versions_post(template_id, template_version_create_request)

Create Template Version

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.template_version_create_request import TemplateVersionCreateRequest
from invoicepdfs.models.template_version_response import TemplateVersionResponse
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
    api_instance = invoicepdfs.TemplateVersionsApi(api_client)
    template_id = 'template_id_example' # str | 
    template_version_create_request = invoicepdfs.TemplateVersionCreateRequest() # TemplateVersionCreateRequest | 

    try:
        # Create Template Version
        api_response = api_instance.create_template_version_api_v1_templates_template_id_versions_post(template_id, template_version_create_request)
        print("The response of TemplateVersionsApi->create_template_version_api_v1_templates_template_id_versions_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplateVersionsApi->create_template_version_api_v1_templates_template_id_versions_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **template_version_create_request** | [**TemplateVersionCreateRequest**](TemplateVersionCreateRequest.md)|  | 

### Return type

[**TemplateVersionResponse**](TemplateVersionResponse.md)

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

# **get_template_version_api_v1_templates_template_id_versions_version_get**
> TemplateVersionResponse get_template_version_api_v1_templates_template_id_versions_version_get(template_id, version)

Get Template Version

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.template_version_response import TemplateVersionResponse
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
    api_instance = invoicepdfs.TemplateVersionsApi(api_client)
    template_id = 'template_id_example' # str | 
    version = 56 # int | 

    try:
        # Get Template Version
        api_response = api_instance.get_template_version_api_v1_templates_template_id_versions_version_get(template_id, version)
        print("The response of TemplateVersionsApi->get_template_version_api_v1_templates_template_id_versions_version_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplateVersionsApi->get_template_version_api_v1_templates_template_id_versions_version_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **version** | **int**|  | 

### Return type

[**TemplateVersionResponse**](TemplateVersionResponse.md)

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

# **list_template_versions_api_v1_templates_template_id_versions_get**
> TemplateVersionsListResponse list_template_versions_api_v1_templates_template_id_versions_get(template_id)

List Template Versions

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.template_versions_list_response import TemplateVersionsListResponse
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
    api_instance = invoicepdfs.TemplateVersionsApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # List Template Versions
        api_response = api_instance.list_template_versions_api_v1_templates_template_id_versions_get(template_id)
        print("The response of TemplateVersionsApi->list_template_versions_api_v1_templates_template_id_versions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplateVersionsApi->list_template_versions_api_v1_templates_template_id_versions_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**TemplateVersionsListResponse**](TemplateVersionsListResponse.md)

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

