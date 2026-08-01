# CreditNotesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CreditNoteOut]**](CreditNoteOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.credit_notes_list_response import CreditNotesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNotesListResponse from a JSON string
credit_notes_list_response_instance = CreditNotesListResponse.from_json(json)
# print the JSON string representation of the object
print(CreditNotesListResponse.to_json())

# convert the object into a dict
credit_notes_list_response_dict = credit_notes_list_response_instance.to_dict()
# create an instance of CreditNotesListResponse from a dict
credit_notes_list_response_from_dict = CreditNotesListResponse.from_dict(credit_notes_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


