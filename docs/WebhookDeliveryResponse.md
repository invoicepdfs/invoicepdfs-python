# WebhookDeliveryResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WebhookDeliveryOut**](WebhookDeliveryOut.md) |  | 

## Example

```python
from invoicepdfs.models.webhook_delivery_response import WebhookDeliveryResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryResponse from a JSON string
webhook_delivery_response_instance = WebhookDeliveryResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryResponse.to_json())

# convert the object into a dict
webhook_delivery_response_dict = webhook_delivery_response_instance.to_dict()
# create an instance of WebhookDeliveryResponse from a dict
webhook_delivery_response_from_dict = WebhookDeliveryResponse.from_dict(webhook_delivery_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


