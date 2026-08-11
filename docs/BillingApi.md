# invoicepdfs.BillingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_checkout_session**](BillingApi.md#create_checkout_session) | **POST** /api/v1/billing/checkout-session | Create Checkout
[**create_portal_session**](BillingApi.md#create_portal_session) | **POST** /api/v1/billing/portal-session | Create Portal
[**get_subscription**](BillingApi.md#get_subscription) | **GET** /api/v1/billing/subscription | Get Subscription
[**list_plans**](BillingApi.md#list_plans) | **GET** /api/v1/billing/plans | List Plans


# **create_checkout_session**
> BillingCheckoutResponse create_checkout_session(billing_checkout_request)

Create Checkout

Create a Stripe Checkout session for a subscription.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.billing_checkout_request import BillingCheckoutRequest
from invoicepdfs.models.billing_checkout_response import BillingCheckoutResponse
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
    api_instance = invoicepdfs.BillingApi(api_client)
    billing_checkout_request = invoicepdfs.BillingCheckoutRequest() # BillingCheckoutRequest | 

    try:
        # Create Checkout
        api_response = api_instance.create_checkout_session(billing_checkout_request)
        print("The response of BillingApi->create_checkout_session:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_checkout_session: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **billing_checkout_request** | [**BillingCheckoutRequest**](BillingCheckoutRequest.md)|  | 

### Return type

[**BillingCheckoutResponse**](BillingCheckoutResponse.md)

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

# **create_portal_session**
> BillingPortalResponse create_portal_session()

Create Portal

Create a Stripe Customer Portal session for self-service management.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.billing_portal_response import BillingPortalResponse
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
    api_instance = invoicepdfs.BillingApi(api_client)

    try:
        # Create Portal
        api_response = api_instance.create_portal_session()
        print("The response of BillingApi->create_portal_session:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_portal_session: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**BillingPortalResponse**](BillingPortalResponse.md)

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

# **get_subscription**
> BillingSubscriptionResponse get_subscription()

Get Subscription

Get current subscription status (from DB, no Stripe API call).

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.billing_subscription_response import BillingSubscriptionResponse
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
    api_instance = invoicepdfs.BillingApi(api_client)

    try:
        # Get Subscription
        api_response = api_instance.get_subscription()
        print("The response of BillingApi->get_subscription:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_subscription: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**BillingSubscriptionResponse**](BillingSubscriptionResponse.md)

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

# **list_plans**
> BillingPlansListResponse list_plans()

List Plans

Purchasable plans — the ones wired to a Stripe price.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.billing_plans_list_response import BillingPlansListResponse
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
    api_instance = invoicepdfs.BillingApi(api_client)

    try:
        # List Plans
        api_response = api_instance.list_plans()
        print("The response of BillingApi->list_plans:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->list_plans: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**BillingPlansListResponse**](BillingPlansListResponse.md)

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

