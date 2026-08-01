# NumberingSequencesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[NumberingSequenceOut]**](NumberingSequenceOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.numbering_sequences_list_response import NumberingSequencesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingSequencesListResponse from a JSON string
numbering_sequences_list_response_instance = NumberingSequencesListResponse.from_json(json)
# print the JSON string representation of the object
print(NumberingSequencesListResponse.to_json())

# convert the object into a dict
numbering_sequences_list_response_dict = numbering_sequences_list_response_instance.to_dict()
# create an instance of NumberingSequencesListResponse from a dict
numbering_sequences_list_response_from_dict = NumberingSequencesListResponse.from_dict(numbering_sequences_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


