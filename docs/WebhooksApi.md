# invoicepdfs.WebhooksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_webhook_endpoint_api_v1_webhook_endpoints_post**](WebhooksApi.md#create_webhook_endpoint_api_v1_webhook_endpoints_post) | **POST** /api/v1/webhook-endpoints | Create Webhook Endpoint
[**delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete**](WebhooksApi.md#delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete) | **DELETE** /api/v1/webhook-endpoints/{endpoint_id} | Delete Webhook Endpoint
[**get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get**](WebhooksApi.md#get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get) | **GET** /api/v1/webhook-deliveries/{delivery_id} | Get Webhook Delivery
[**get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get**](WebhooksApi.md#get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get) | **GET** /api/v1/webhook-endpoints/{endpoint_id} | Get Webhook Endpoint
[**list_webhook_deliveries_api_v1_webhook_deliveries_get**](WebhooksApi.md#list_webhook_deliveries_api_v1_webhook_deliveries_get) | **GET** /api/v1/webhook-deliveries | List Webhook Deliveries
[**list_webhook_endpoints_api_v1_webhook_endpoints_get**](WebhooksApi.md#list_webhook_endpoints_api_v1_webhook_endpoints_get) | **GET** /api/v1/webhook-endpoints | List Webhook Endpoints
[**retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post**](WebhooksApi.md#retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post) | **POST** /api/v1/webhook-deliveries/{delivery_id}/retry | Retry Webhook Delivery
[**rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post**](WebhooksApi.md#rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post) | **POST** /api/v1/webhook-endpoints/{endpoint_id}/rotate-secret | Rotate Webhook Secret
[**test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post**](WebhooksApi.md#test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post) | **POST** /api/v1/webhook-endpoints/{endpoint_id}/test | Test Webhook Endpoint
[**update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch**](WebhooksApi.md#update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch) | **PATCH** /api/v1/webhook-endpoints/{endpoint_id} | Update Webhook Endpoint


# **create_webhook_endpoint_api_v1_webhook_endpoints_post**
> WebhookEndpointResponse create_webhook_endpoint_api_v1_webhook_endpoints_post(webhook_endpoint_create_request)

Create Webhook Endpoint

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_endpoint_create_request import WebhookEndpointCreateRequest
from invoicepdfs.models.webhook_endpoint_response import WebhookEndpointResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    webhook_endpoint_create_request = invoicepdfs.WebhookEndpointCreateRequest() # WebhookEndpointCreateRequest | 

    try:
        # Create Webhook Endpoint
        api_response = api_instance.create_webhook_endpoint_api_v1_webhook_endpoints_post(webhook_endpoint_create_request)
        print("The response of WebhooksApi->create_webhook_endpoint_api_v1_webhook_endpoints_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->create_webhook_endpoint_api_v1_webhook_endpoints_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhook_endpoint_create_request** | [**WebhookEndpointCreateRequest**](WebhookEndpointCreateRequest.md)|  | 

### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

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

# **delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete**
> SimpleBoolResponse delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete(endpoint_id)

Delete Webhook Endpoint

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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    endpoint_id = 'endpoint_id_example' # str | 

    try:
        # Delete Webhook Endpoint
        api_response = api_instance.delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete(endpoint_id)
        print("The response of WebhooksApi->delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->delete_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endpoint_id** | **str**|  | 

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

# **get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get**
> WebhookDeliveryResponse get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get(delivery_id)

Get Webhook Delivery

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_delivery_response import WebhookDeliveryResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    delivery_id = 'delivery_id_example' # str | 

    try:
        # Get Webhook Delivery
        api_response = api_instance.get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get(delivery_id)
        print("The response of WebhooksApi->get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_webhook_delivery_api_v1_webhook_deliveries_delivery_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_id** | **str**|  | 

### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

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

# **get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get**
> WebhookEndpointResponse get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get(endpoint_id)

Get Webhook Endpoint

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_endpoint_response import WebhookEndpointResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    endpoint_id = 'endpoint_id_example' # str | 

    try:
        # Get Webhook Endpoint
        api_response = api_instance.get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get(endpoint_id)
        print("The response of WebhooksApi->get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endpoint_id** | **str**|  | 

### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

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

# **list_webhook_deliveries_api_v1_webhook_deliveries_get**
> WebhookDeliveriesListResponse list_webhook_deliveries_api_v1_webhook_deliveries_get(limit=limit, cursor=cursor)

List Webhook Deliveries

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_deliveries_list_response import WebhookDeliveriesListResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Webhook Deliveries
        api_response = api_instance.list_webhook_deliveries_api_v1_webhook_deliveries_get(limit=limit, cursor=cursor)
        print("The response of WebhooksApi->list_webhook_deliveries_api_v1_webhook_deliveries_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->list_webhook_deliveries_api_v1_webhook_deliveries_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**WebhookDeliveriesListResponse**](WebhookDeliveriesListResponse.md)

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

# **list_webhook_endpoints_api_v1_webhook_endpoints_get**
> WebhookEndpointsListResponse list_webhook_endpoints_api_v1_webhook_endpoints_get(limit=limit, cursor=cursor)

List Webhook Endpoints

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_endpoints_list_response import WebhookEndpointsListResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List Webhook Endpoints
        api_response = api_instance.list_webhook_endpoints_api_v1_webhook_endpoints_get(limit=limit, cursor=cursor)
        print("The response of WebhooksApi->list_webhook_endpoints_api_v1_webhook_endpoints_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->list_webhook_endpoints_api_v1_webhook_endpoints_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 

### Return type

[**WebhookEndpointsListResponse**](WebhookEndpointsListResponse.md)

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

# **retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post**
> WebhookDeliveryResponse retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post(delivery_id)

Retry Webhook Delivery

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_delivery_response import WebhookDeliveryResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    delivery_id = 'delivery_id_example' # str | 

    try:
        # Retry Webhook Delivery
        api_response = api_instance.retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post(delivery_id)
        print("The response of WebhooksApi->retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->retry_webhook_delivery_api_v1_webhook_deliveries_delivery_id_retry_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_id** | **str**|  | 

### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

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

# **rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post**
> WebhookSecretResponse rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post(endpoint_id)

Rotate Webhook Secret

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_secret_response import WebhookSecretResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    endpoint_id = 'endpoint_id_example' # str | 

    try:
        # Rotate Webhook Secret
        api_response = api_instance.rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post(endpoint_id)
        print("The response of WebhooksApi->rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->rotate_webhook_secret_api_v1_webhook_endpoints_endpoint_id_rotate_secret_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endpoint_id** | **str**|  | 

### Return type

[**WebhookSecretResponse**](WebhookSecretResponse.md)

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

# **test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post**
> WebhookDeliveryResponse test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post(endpoint_id)

Test Webhook Endpoint

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_delivery_response import WebhookDeliveryResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    endpoint_id = 'endpoint_id_example' # str | 

    try:
        # Test Webhook Endpoint
        api_response = api_instance.test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post(endpoint_id)
        print("The response of WebhooksApi->test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->test_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_test_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endpoint_id** | **str**|  | 

### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

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

# **update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch**
> WebhookEndpointResponse update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch(endpoint_id, webhook_endpoint_patch_request)

Update Webhook Endpoint

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.webhook_endpoint_patch_request import WebhookEndpointPatchRequest
from invoicepdfs.models.webhook_endpoint_response import WebhookEndpointResponse
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
    api_instance = invoicepdfs.WebhooksApi(api_client)
    endpoint_id = 'endpoint_id_example' # str | 
    webhook_endpoint_patch_request = invoicepdfs.WebhookEndpointPatchRequest() # WebhookEndpointPatchRequest | 

    try:
        # Update Webhook Endpoint
        api_response = api_instance.update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch(endpoint_id, webhook_endpoint_patch_request)
        print("The response of WebhooksApi->update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->update_webhook_endpoint_api_v1_webhook_endpoints_endpoint_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endpoint_id** | **str**|  | 
 **webhook_endpoint_patch_request** | [**WebhookEndpointPatchRequest**](WebhookEndpointPatchRequest.md)|  | 

### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

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

