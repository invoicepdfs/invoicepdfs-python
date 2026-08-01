# InvoiceNoteInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**content** | **str** |  | 

## Example

```python
from invoicepdfs.models.invoice_note_input import InvoiceNoteInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceNoteInput from a JSON string
invoice_note_input_instance = InvoiceNoteInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceNoteInput.to_json())

# convert the object into a dict
invoice_note_input_dict = invoice_note_input_instance.to_dict()
# create an instance of InvoiceNoteInput from a dict
invoice_note_input_from_dict = InvoiceNoteInput.from_dict(invoice_note_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


