# invoicepdfs.TemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_template_api_v1_templates_custom_post**](TemplatesApi.md#create_template_api_v1_templates_custom_post) | **POST** /api/v1/templates/custom | Create Template
[**delete_template_api_v1_templates_custom_template_id_delete**](TemplatesApi.md#delete_template_api_v1_templates_custom_template_id_delete) | **DELETE** /api/v1/templates/custom/{template_id} | Delete Template
[**duplicate_template_api_v1_templates_custom_template_id_duplicate_post**](TemplatesApi.md#duplicate_template_api_v1_templates_custom_template_id_duplicate_post) | **POST** /api/v1/templates/custom/{template_id}/duplicate | Duplicate Template
[**get_builtin_template_api_v1_templates_builtin_template_id_get**](TemplatesApi.md#get_builtin_template_api_v1_templates_builtin_template_id_get) | **GET** /api/v1/templates/builtin/{template_id} | Get Builtin Template
[**get_custom_template_api_v1_templates_custom_template_id_get**](TemplatesApi.md#get_custom_template_api_v1_templates_custom_template_id_get) | **GET** /api/v1/templates/custom/{template_id} | Get Custom Template
[**get_template_api_v1_templates_template_id_get**](TemplatesApi.md#get_template_api_v1_templates_template_id_get) | **GET** /api/v1/templates/{template_id} | Get Template
[**list_custom_templates_api_v1_templates_custom_get**](TemplatesApi.md#list_custom_templates_api_v1_templates_custom_get) | **GET** /api/v1/templates/custom | List Custom Templates
[**patch_template_api_v1_templates_custom_template_id_patch**](TemplatesApi.md#patch_template_api_v1_templates_custom_template_id_patch) | **PATCH** /api/v1/templates/custom/{template_id} | Patch Template
[**preview_template_api_v1_templates_template_id_preview_post**](TemplatesApi.md#preview_template_api_v1_templates_template_id_preview_post) | **POST** /api/v1/templates/{template_id}/preview | Preview Template
[**publish_template_api_v1_templates_custom_template_id_publish_post**](TemplatesApi.md#publish_template_api_v1_templates_custom_template_id_publish_post) | **POST** /api/v1/templates/custom/{template_id}/publish | Publish Template
[**templates_api_v1_templates_get**](TemplatesApi.md#templates_api_v1_templates_get) | **GET** /api/v1/templates | Templates


# **create_template_api_v1_templates_custom_post**
> CustomTemplateResponse create_template_api_v1_templates_custom_post(template_create_request)

Create Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_template_response import CustomTemplateResponse
from invoicepdfs.models.template_create_request import TemplateCreateRequest
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_create_request = invoicepdfs.TemplateCreateRequest() # TemplateCreateRequest | 

    try:
        # Create Template
        api_response = api_instance.create_template_api_v1_templates_custom_post(template_create_request)
        print("The response of TemplatesApi->create_template_api_v1_templates_custom_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->create_template_api_v1_templates_custom_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_create_request** | [**TemplateCreateRequest**](TemplateCreateRequest.md)|  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_template_api_v1_templates_custom_template_id_delete**
> delete_template_api_v1_templates_custom_template_id_delete(template_id)

Delete Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Delete Template
        api_instance.delete_template_api_v1_templates_custom_template_id_delete(template_id)
    except Exception as e:
        print("Exception when calling TemplatesApi->delete_template_api_v1_templates_custom_template_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **duplicate_template_api_v1_templates_custom_template_id_duplicate_post**
> CustomTemplateResponse duplicate_template_api_v1_templates_custom_template_id_duplicate_post(template_id)

Duplicate Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_template_response import CustomTemplateResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Duplicate Template
        api_response = api_instance.duplicate_template_api_v1_templates_custom_template_id_duplicate_post(template_id)
        print("The response of TemplatesApi->duplicate_template_api_v1_templates_custom_template_id_duplicate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->duplicate_template_api_v1_templates_custom_template_id_duplicate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_builtin_template_api_v1_templates_builtin_template_id_get**
> TemplateDetailResponse get_builtin_template_api_v1_templates_builtin_template_id_get(template_id)

Get Builtin Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.template_detail_response import TemplateDetailResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Get Builtin Template
        api_response = api_instance.get_builtin_template_api_v1_templates_builtin_template_id_get(template_id)
        print("The response of TemplatesApi->get_builtin_template_api_v1_templates_builtin_template_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->get_builtin_template_api_v1_templates_builtin_template_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**TemplateDetailResponse**](TemplateDetailResponse.md)

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

# **get_custom_template_api_v1_templates_custom_template_id_get**
> CustomTemplateResponse get_custom_template_api_v1_templates_custom_template_id_get(template_id)

Get Custom Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_template_response import CustomTemplateResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Get Custom Template
        api_response = api_instance.get_custom_template_api_v1_templates_custom_template_id_get(template_id)
        print("The response of TemplatesApi->get_custom_template_api_v1_templates_custom_template_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->get_custom_template_api_v1_templates_custom_template_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

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

# **get_template_api_v1_templates_template_id_get**
> TemplateDetailResponse get_template_api_v1_templates_template_id_get(template_id)

Get Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.template_detail_response import TemplateDetailResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Get Template
        api_response = api_instance.get_template_api_v1_templates_template_id_get(template_id)
        print("The response of TemplatesApi->get_template_api_v1_templates_template_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->get_template_api_v1_templates_template_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**TemplateDetailResponse**](TemplateDetailResponse.md)

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

# **list_custom_templates_api_v1_templates_custom_get**
> CustomTemplatesListResponse list_custom_templates_api_v1_templates_custom_get(limit=limit, cursor=cursor)

List Custom Templates

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_templates_list_response import CustomTemplatesListResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Custom Templates
        api_response = api_instance.list_custom_templates_api_v1_templates_custom_get(limit=limit, cursor=cursor)
        print("The response of TemplatesApi->list_custom_templates_api_v1_templates_custom_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->list_custom_templates_api_v1_templates_custom_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**CustomTemplatesListResponse**](CustomTemplatesListResponse.md)

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

# **patch_template_api_v1_templates_custom_template_id_patch**
> CustomTemplateResponse patch_template_api_v1_templates_custom_template_id_patch(template_id, template_patch_request)

Patch Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_template_response import CustomTemplateResponse
from invoicepdfs.models.template_patch_request import TemplatePatchRequest
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 
    template_patch_request = invoicepdfs.TemplatePatchRequest() # TemplatePatchRequest | 

    try:
        # Patch Template
        api_response = api_instance.patch_template_api_v1_templates_custom_template_id_patch(template_id, template_patch_request)
        print("The response of TemplatesApi->patch_template_api_v1_templates_custom_template_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->patch_template_api_v1_templates_custom_template_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **template_patch_request** | [**TemplatePatchRequest**](TemplatePatchRequest.md)|  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

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

# **preview_template_api_v1_templates_template_id_preview_post**
> object preview_template_api_v1_templates_template_id_preview_post(template_id, document_render_request, idempotency_key=idempotency_key)

Preview Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_render_request import DocumentRenderRequest
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 
    document_render_request = invoicepdfs.DocumentRenderRequest() # DocumentRenderRequest | 
    idempotency_key = 'idempotency_key_example' # str |  (optional)

    try:
        # Preview Template
        api_response = api_instance.preview_template_api_v1_templates_template_id_preview_post(template_id, document_render_request, idempotency_key=idempotency_key)
        print("The response of TemplatesApi->preview_template_api_v1_templates_template_id_preview_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->preview_template_api_v1_templates_template_id_preview_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **document_render_request** | [**DocumentRenderRequest**](DocumentRenderRequest.md)|  | 
 **idempotency_key** | **str**|  | [optional] 

### Return type

**object**

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

# **publish_template_api_v1_templates_custom_template_id_publish_post**
> CustomTemplateResponse publish_template_api_v1_templates_custom_template_id_publish_post(template_id)

Publish Template

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.custom_template_response import CustomTemplateResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)
    template_id = 'template_id_example' # str | 

    try:
        # Publish Template
        api_response = api_instance.publish_template_api_v1_templates_custom_template_id_publish_post(template_id)
        print("The response of TemplatesApi->publish_template_api_v1_templates_custom_template_id_publish_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->publish_template_api_v1_templates_custom_template_id_publish_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

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

# **templates_api_v1_templates_get**
> TemplatesListResponse templates_api_v1_templates_get()

Templates

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.templates_list_response import TemplatesListResponse
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
    api_instance = invoicepdfs.TemplatesApi(api_client)

    try:
        # Templates
        api_response = api_instance.templates_api_v1_templates_get()
        print("The response of TemplatesApi->templates_api_v1_templates_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TemplatesApi->templates_api_v1_templates_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TemplatesListResponse**](TemplatesListResponse.md)

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

