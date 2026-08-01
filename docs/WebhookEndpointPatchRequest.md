# WebhookEndpointPatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**events** | **List[str]** |  | [optional] 
**is_active** | **bool** |  | [optional] 

## Example

```python
from invoicepdfs.models.webhook_endpoint_patch_request import WebhookEndpointPatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEndpointPatchRequest from a JSON string
webhook_endpoint_patch_request_instance = WebhookEndpointPatchRequest.from_json(json)
# print the JSON string representation of the object
print(WebhookEndpointPatchRequest.to_json())

# convert the object into a dict
webhook_endpoint_patch_request_dict = webhook_endpoint_patch_request_instance.to_dict()
# create an instance of WebhookEndpointPatchRequest from a dict
webhook_endpoint_patch_request_from_dict = WebhookEndpointPatchRequest.from_dict(webhook_endpoint_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


