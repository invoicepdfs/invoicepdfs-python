# CreditNoteOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**invoice_id** | **str** |  | 
**credit_note_number** | **str** |  | 
**status** | **str** |  | 
**reason** | **str** |  | [optional] 
**currency** | **str** |  | 
**totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**issue_date** | **date** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**finalized_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.credit_note_out import CreditNoteOut

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNoteOut from a JSON string
credit_note_out_instance = CreditNoteOut.from_json(json)
# print the JSON string representation of the object
print(CreditNoteOut.to_json())

# convert the object into a dict
credit_note_out_dict = credit_note_out_instance.to_dict()
# create an instance of CreditNoteOut from a dict
credit_note_out_from_dict = CreditNoteOut.from_dict(credit_note_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


