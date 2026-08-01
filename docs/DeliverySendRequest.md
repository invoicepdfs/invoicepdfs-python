# DeliverySendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | **List[str]** |  | 
**cc** | **List[str]** |  | [optional] 
**bcc** | **List[str]** |  | [optional] 
**subject** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**attach_pdf** | **bool** |  | [optional] [default to True]

## Example

```python
from invoicepdfs.models.delivery_send_request import DeliverySendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DeliverySendRequest from a JSON string
delivery_send_request_instance = DeliverySendRequest.from_json(json)
# print the JSON string representation of the object
print(DeliverySendRequest.to_json())

# convert the object into a dict
delivery_send_request_dict = delivery_send_request_instance.to_dict()
# create an instance of DeliverySendRequest from a dict
delivery_send_request_from_dict = DeliverySendRequest.from_dict(delivery_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


