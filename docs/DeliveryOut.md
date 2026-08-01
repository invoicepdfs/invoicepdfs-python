# DeliveryOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**invoice_id** | **str** |  | 
**to** | **List[str]** |  | 
**cc** | **List[str]** |  | 
**bcc** | **List[str]** |  | 
**subject** | **str** |  | 
**message** | **str** |  | [optional] 
**attach_pdf** | **bool** |  | 
**status** | **str** |  | 
**created_at** | **str** |  | 
**sent_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.delivery_out import DeliveryOut

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryOut from a JSON string
delivery_out_instance = DeliveryOut.from_json(json)
# print the JSON string representation of the object
print(DeliveryOut.to_json())

# convert the object into a dict
delivery_out_dict = delivery_out_instance.to_dict()
# create an instance of DeliveryOut from a dict
delivery_out_from_dict = DeliveryOut.from_dict(delivery_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


