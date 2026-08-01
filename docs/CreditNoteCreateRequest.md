# CreditNoteCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_id** | **str** |  | 
**credit_note_number** | **str** |  | 
**issue_date** | **date** |  | 
**reason** | **str** |  | [optional] 
**line_items** | [**List[CreditNoteLineItemInput]**](CreditNoteLineItemInput.md) |  | 

## Example

```python
from invoicepdfs.models.credit_note_create_request import CreditNoteCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNoteCreateRequest from a JSON string
credit_note_create_request_instance = CreditNoteCreateRequest.from_json(json)
# print the JSON string representation of the object
print(CreditNoteCreateRequest.to_json())

# convert the object into a dict
credit_note_create_request_dict = credit_note_create_request_instance.to_dict()
# create an instance of CreditNoteCreateRequest from a dict
credit_note_create_request_from_dict = CreditNoteCreateRequest.from_dict(credit_note_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


