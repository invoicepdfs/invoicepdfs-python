# PaymentCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**paid_at** | **datetime** |  | 
**method** | **str** |  | [optional] 
**reference** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.payment_create_request import PaymentCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentCreateRequest from a JSON string
payment_create_request_instance = PaymentCreateRequest.from_json(json)
# print the JSON string representation of the object
print(PaymentCreateRequest.to_json())

# convert the object into a dict
payment_create_request_dict = payment_create_request_instance.to_dict()
# create an instance of PaymentCreateRequest from a dict
payment_create_request_from_dict = PaymentCreateRequest.from_dict(payment_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


