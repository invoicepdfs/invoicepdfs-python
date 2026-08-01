# WebhookDeliveryOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**endpoint_id** | **str** |  | 
**event_id** | **str** |  | 
**event_type** | **str** |  | 
**status** | **str** |  | 
**http_status** | **int** |  | [optional] 
**attempts** | **int** |  | 
**error_message** | **str** |  | [optional] 
**created_at** | **str** |  | 
**delivered_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.webhook_delivery_out import WebhookDeliveryOut

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryOut from a JSON string
webhook_delivery_out_instance = WebhookDeliveryOut.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryOut.to_json())

# convert the object into a dict
webhook_delivery_out_dict = webhook_delivery_out_instance.to_dict()
# create an instance of WebhookDeliveryOut from a dict
webhook_delivery_out_from_dict = WebhookDeliveryOut.from_dict(webhook_delivery_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


