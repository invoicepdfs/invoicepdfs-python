# NumberingSequencePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**prefix** | **str** |  | [optional] 
**date_pattern** | **str** |  | [optional] 
**padding** | **int** |  | [optional] 
**next_number** | **int** |  | [optional] 
**reset** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.numbering_sequence_patch_request import NumberingSequencePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingSequencePatchRequest from a JSON string
numbering_sequence_patch_request_instance = NumberingSequencePatchRequest.from_json(json)
# print the JSON string representation of the object
print(NumberingSequencePatchRequest.to_json())

# convert the object into a dict
numbering_sequence_patch_request_dict = numbering_sequence_patch_request_instance.to_dict()
# create an instance of NumberingSequencePatchRequest from a dict
numbering_sequence_patch_request_from_dict = NumberingSequencePatchRequest.from_dict(numbering_sequence_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


