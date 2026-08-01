# WebhookEndpointOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**url** | **str** |  | 
**description** | **str** |  | [optional] 
**events** | **List[str]** |  | 
**is_active** | **bool** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.webhook_endpoint_out import WebhookEndpointOut

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEndpointOut from a JSON string
webhook_endpoint_out_instance = WebhookEndpointOut.from_json(json)
# print the JSON string representation of the object
print(WebhookEndpointOut.to_json())

# convert the object into a dict
webhook_endpoint_out_dict = webhook_endpoint_out_instance.to_dict()
# create an instance of WebhookEndpointOut from a dict
webhook_endpoint_out_from_dict = WebhookEndpointOut.from_dict(webhook_endpoint_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


