# InvoiceLineItemTaxInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tax_rate_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**rate** | **str** |  | [optional] 
**inclusive** | **bool** |  | [optional] [default to False]

## Example

```python
from invoicepdfs.models.invoice_line_item_tax_input import InvoiceLineItemTaxInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceLineItemTaxInput from a JSON string
invoice_line_item_tax_input_instance = InvoiceLineItemTaxInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceLineItemTaxInput.to_json())

# convert the object into a dict
invoice_line_item_tax_input_dict = invoice_line_item_tax_input_instance.to_dict()
# create an instance of InvoiceLineItemTaxInput from a dict
invoice_line_item_tax_input_from_dict = InvoiceLineItemTaxInput.from_dict(invoice_line_item_tax_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


