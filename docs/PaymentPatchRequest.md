# PaymentPatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | [optional] 
**paid_at** | **datetime** |  | [optional] 
**method** | **str** |  | [optional] 
**reference** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.payment_patch_request import PaymentPatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentPatchRequest from a JSON string
payment_patch_request_instance = PaymentPatchRequest.from_json(json)
# print the JSON string representation of the object
print(PaymentPatchRequest.to_json())

# convert the object into a dict
payment_patch_request_dict = payment_patch_request_instance.to_dict()
# create an instance of PaymentPatchRequest from a dict
payment_patch_request_from_dict = PaymentPatchRequest.from_dict(payment_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


