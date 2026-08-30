# InvoiceShippingInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] [default to 'Shipping']
**amount** | **str** |  | 
**taxable** | **bool** |  | [optional] [default to False]

## Example

```python
from invoicepdfs.models.invoice_shipping_input import InvoiceShippingInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceShippingInput from a JSON string
invoice_shipping_input_instance = InvoiceShippingInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceShippingInput.to_json())

# convert the object into a dict
invoice_shipping_input_dict = invoice_shipping_input_instance.to_dict()
# create an instance of InvoiceShippingInput from a dict
invoice_shipping_input_from_dict = InvoiceShippingInput.from_dict(invoice_shipping_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


