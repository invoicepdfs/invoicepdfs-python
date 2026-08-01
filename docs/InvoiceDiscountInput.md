# InvoiceDiscountInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] [default to 'percentage']
**value** | **str** |  | 
**reason** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_discount_input import InvoiceDiscountInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceDiscountInput from a JSON string
invoice_discount_input_instance = InvoiceDiscountInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceDiscountInput.to_json())

# convert the object into a dict
invoice_discount_input_dict = invoice_discount_input_instance.to_dict()
# create an instance of InvoiceDiscountInput from a dict
invoice_discount_input_from_dict = InvoiceDiscountInput.from_dict(invoice_discount_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


