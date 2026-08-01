# CreditNoteResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CreditNoteOut**](CreditNoteOut.md) |  | 

## Example

```python
from invoicepdfs.models.credit_note_response import CreditNoteResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNoteResponse from a JSON string
credit_note_response_instance = CreditNoteResponse.from_json(json)
# print the JSON string representation of the object
print(CreditNoteResponse.to_json())

# convert the object into a dict
credit_note_response_dict = credit_note_response_instance.to_dict()
# create an instance of CreditNoteResponse from a dict
credit_note_response_from_dict = CreditNoteResponse.from_dict(credit_note_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


