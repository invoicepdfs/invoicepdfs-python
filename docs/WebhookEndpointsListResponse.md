# WebhookEndpointsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WebhookEndpointOut]**](WebhookEndpointOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.webhook_endpoints_list_response import WebhookEndpointsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEndpointsListResponse from a JSON string
webhook_endpoints_list_response_instance = WebhookEndpointsListResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookEndpointsListResponse.to_json())

# convert the object into a dict
webhook_endpoints_list_response_dict = webhook_endpoints_list_response_instance.to_dict()
# create an instance of WebhookEndpointsListResponse from a dict
webhook_endpoints_list_response_from_dict = WebhookEndpointsListResponse.from_dict(webhook_endpoints_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


