# invoicepdfs.JobsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_job_api_v1_jobs_job_id_cancel_post**](JobsApi.md#cancel_job_api_v1_jobs_job_id_cancel_post) | **POST** /api/v1/jobs/{job_id}/cancel | Cancel Job
[**get_job_api_v1_jobs_job_id_get**](JobsApi.md#get_job_api_v1_jobs_job_id_get) | **GET** /api/v1/jobs/{job_id} | Get Job
[**retry_job_api_v1_jobs_job_id_retry_post**](JobsApi.md#retry_job_api_v1_jobs_job_id_retry_post) | **POST** /api/v1/jobs/{job_id}/retry | Retry Job


# **cancel_job_api_v1_jobs_job_id_cancel_post**
> JobResponse cancel_job_api_v1_jobs_job_id_cancel_post(job_id)

Cancel Job

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.job_response import JobResponse
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
    api_instance = invoicepdfs.JobsApi(api_client)
    job_id = 'job_id_example' # str | 

    try:
        # Cancel Job
        api_response = api_instance.cancel_job_api_v1_jobs_job_id_cancel_post(job_id)
        print("The response of JobsApi->cancel_job_api_v1_jobs_job_id_cancel_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->cancel_job_api_v1_jobs_job_id_cancel_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 

### Return type

[**JobResponse**](JobResponse.md)

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

# **get_job_api_v1_jobs_job_id_get**
> JobResponse get_job_api_v1_jobs_job_id_get(job_id)

Get Job

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.job_response import JobResponse
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
    api_instance = invoicepdfs.JobsApi(api_client)
    job_id = 'job_id_example' # str | 

    try:
        # Get Job
        api_response = api_instance.get_job_api_v1_jobs_job_id_get(job_id)
        print("The response of JobsApi->get_job_api_v1_jobs_job_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->get_job_api_v1_jobs_job_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 

### Return type

[**JobResponse**](JobResponse.md)

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

# **retry_job_api_v1_jobs_job_id_retry_post**
> JobResponse retry_job_api_v1_jobs_job_id_retry_post(job_id)

Retry Job

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.job_response import JobResponse
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
    api_instance = invoicepdfs.JobsApi(api_client)
    job_id = 'job_id_example' # str | 

    try:
        # Retry Job
        api_response = api_instance.retry_job_api_v1_jobs_job_id_retry_post(job_id)
        print("The response of JobsApi->retry_job_api_v1_jobs_job_id_retry_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobsApi->retry_job_api_v1_jobs_job_id_retry_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 

### Return type

[**JobResponse**](JobResponse.md)

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

