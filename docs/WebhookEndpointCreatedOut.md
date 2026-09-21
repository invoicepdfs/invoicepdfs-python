# WebhookEndpointCreatedOut

A newly created endpoint, including its signing secret.  The only time the secret is returned. Store it now: reading or listing endpoints never includes it, and the only way to obtain another is to rotate, which invalidates this one.

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
**secret** | **str** |  | 

## Example

```python
from invoicepdfs.models.webhook_endpoint_created_out import WebhookEndpointCreatedOut

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEndpointCreatedOut from a JSON string
webhook_endpoint_created_out_instance = WebhookEndpointCreatedOut.from_json(json)
# print the JSON string representation of the object
print(WebhookEndpointCreatedOut.to_json())

# convert the object into a dict
webhook_endpoint_created_out_dict = webhook_endpoint_created_out_instance.to_dict()
# create an instance of WebhookEndpointCreatedOut from a dict
webhook_endpoint_created_out_from_dict = WebhookEndpointCreatedOut.from_dict(webhook_endpoint_created_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


