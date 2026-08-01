# InvoiceLineItemInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**quantity** | **str** | Decimal string | 
**unit_price** | **str** | Decimal string in major units | 
**unit** | **str** |  | [optional] 
**sku** | **str** |  | [optional] 
**discount** | [**InvoiceDiscountInput**](InvoiceDiscountInput.md) |  | [optional] 
**taxes** | [**List[InvoiceLineItemTaxInput]**](InvoiceLineItemTaxInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_line_item_input import InvoiceLineItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceLineItemInput from a JSON string
invoice_line_item_input_instance = InvoiceLineItemInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceLineItemInput.to_json())

# convert the object into a dict
invoice_line_item_input_dict = invoice_line_item_input_instance.to_dict()
# create an instance of InvoiceLineItemInput from a dict
invoice_line_item_input_from_dict = InvoiceLineItemInput.from_dict(invoice_line_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


