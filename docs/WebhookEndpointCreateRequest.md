# WebhookEndpointCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | 
**description** | **str** |  | [optional] 
**events** | **List[str]** |  | 

## Example

```python
from invoicepdfs.models.webhook_endpoint_create_request import WebhookEndpointCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEndpointCreateRequest from a JSON string
webhook_endpoint_create_request_instance = WebhookEndpointCreateRequest.from_json(json)
# print the JSON string representation of the object
print(WebhookEndpointCreateRequest.to_json())

# convert the object into a dict
webhook_endpoint_create_request_dict = webhook_endpoint_create_request_instance.to_dict()
# create an instance of WebhookEndpointCreateRequest from a dict
webhook_endpoint_create_request_from_dict = WebhookEndpointCreateRequest.from_dict(webhook_endpoint_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


