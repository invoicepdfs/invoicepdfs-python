# invoicepdfs.LogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_logs_api_v1_logs_get**](LogsApi.md#list_logs_api_v1_logs_get) | **GET** /api/v1/logs | List Logs


# **list_logs_api_v1_logs_get**
> ApiRequestLogsListResponse list_logs_api_v1_logs_get(status=status, limit=limit)

List Logs

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.api_request_logs_list_response import ApiRequestLogsListResponse
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
    api_instance = invoicepdfs.LogsApi(api_client)
    status = '' # str |  (optional) (default to '')
    limit = 100 # int |  (optional) (default to 100)

    try:
        # List Logs
        api_response = api_instance.list_logs_api_v1_logs_get(status=status, limit=limit)
        print("The response of LogsApi->list_logs_api_v1_logs_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LogsApi->list_logs_api_v1_logs_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **str**|  | [optional] [default to &#39;&#39;]
 **limit** | **int**|  | [optional] [default to 100]

### Return type

[**ApiRequestLogsListResponse**](ApiRequestLogsListResponse.md)

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

