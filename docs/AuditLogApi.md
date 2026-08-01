# invoicepdfs.AuditLogApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_audit_event_api_v1_audit_events_audit_event_id_get**](AuditLogApi.md#get_audit_event_api_v1_audit_events_audit_event_id_get) | **GET** /api/v1/audit-events/{audit_event_id} | Get Audit Event
[**list_audit_events_api_v1_audit_events_get**](AuditLogApi.md#list_audit_events_api_v1_audit_events_get) | **GET** /api/v1/audit-events | List Audit Events


# **get_audit_event_api_v1_audit_events_audit_event_id_get**
> AuditEventResponse get_audit_event_api_v1_audit_events_audit_event_id_get(audit_event_id)

Get Audit Event

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.audit_event_response import AuditEventResponse
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
    api_instance = invoicepdfs.AuditLogApi(api_client)
    audit_event_id = 'audit_event_id_example' # str | 

    try:
        # Get Audit Event
        api_response = api_instance.get_audit_event_api_v1_audit_events_audit_event_id_get(audit_event_id)
        print("The response of AuditLogApi->get_audit_event_api_v1_audit_events_audit_event_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuditLogApi->get_audit_event_api_v1_audit_events_audit_event_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **audit_event_id** | **str**|  | 

### Return type

[**AuditEventResponse**](AuditEventResponse.md)

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

# **list_audit_events_api_v1_audit_events_get**
> AuditEventsListResponse list_audit_events_api_v1_audit_events_get(limit=limit, cursor=cursor, action=action, resource_type=resource_type, resource_id=resource_id)

List Audit Events

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.audit_events_list_response import AuditEventsListResponse
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
    api_instance = invoicepdfs.AuditLogApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    cursor = 'cursor_example' # str |  (optional)
    action = 'action_example' # str |  (optional)
    resource_type = 'resource_type_example' # str |  (optional)
    resource_id = 'resource_id_example' # str |  (optional)

    try:
        # List Audit Events
        api_response = api_instance.list_audit_events_api_v1_audit_events_get(limit=limit, cursor=cursor, action=action, resource_type=resource_type, resource_id=resource_id)
        print("The response of AuditLogApi->list_audit_events_api_v1_audit_events_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuditLogApi->list_audit_events_api_v1_audit_events_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **cursor** | **str**|  | [optional] 
 **action** | **str**|  | [optional] 
 **resource_type** | **str**|  | [optional] 
 **resource_id** | **str**|  | [optional] 

### Return type

[**AuditEventsListResponse**](AuditEventsListResponse.md)

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

