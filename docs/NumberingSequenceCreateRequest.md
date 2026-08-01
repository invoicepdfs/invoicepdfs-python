# NumberingSequenceCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**document_type** | **str** |  | [optional] [default to 'invoice']
**prefix** | **str** |  | [optional] [default to 'INV-']
**date_pattern** | **str** |  | [optional] [default to '{YYYY}-']
**padding** | **int** |  | [optional] [default to 5]
**next_number** | **int** |  | [optional] [default to 1]
**reset** | **str** |  | [optional] [default to 'yearly']

## Example

```python
from invoicepdfs.models.numbering_sequence_create_request import NumberingSequenceCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingSequenceCreateRequest from a JSON string
numbering_sequence_create_request_instance = NumberingSequenceCreateRequest.from_json(json)
# print the JSON string representation of the object
print(NumberingSequenceCreateRequest.to_json())

# convert the object into a dict
numbering_sequence_create_request_dict = numbering_sequence_create_request_instance.to_dict()
# create an instance of NumberingSequenceCreateRequest from a dict
numbering_sequence_create_request_from_dict = NumberingSequenceCreateRequest.from_dict(numbering_sequence_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


