# PaymentOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**invoice_id** | **str** |  | 
**amount** | [**MoneyOut**](MoneyOut.md) |  | 
**paid_at** | **str** |  | 
**method** | **str** |  | [optional] 
**reference** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.payment_out import PaymentOut

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentOut from a JSON string
payment_out_instance = PaymentOut.from_json(json)
# print the JSON string representation of the object
print(PaymentOut.to_json())

# convert the object into a dict
payment_out_dict = payment_out_instance.to_dict()
# create an instance of PaymentOut from a dict
payment_out_from_dict = PaymentOut.from_dict(payment_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


