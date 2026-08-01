# CreditNoteLineItemInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**quantity** | **str** |  | 
**unit_price** | **str** |  | 
**taxes** | [**List[InvoiceLineItemTaxInput]**](InvoiceLineItemTaxInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.credit_note_line_item_input import CreditNoteLineItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNoteLineItemInput from a JSON string
credit_note_line_item_input_instance = CreditNoteLineItemInput.from_json(json)
# print the JSON string representation of the object
print(CreditNoteLineItemInput.to_json())

# convert the object into a dict
credit_note_line_item_input_dict = credit_note_line_item_input_instance.to_dict()
# create an instance of CreditNoteLineItemInput from a dict
credit_note_line_item_input_from_dict = CreditNoteLineItemInput.from_dict(credit_note_line_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


