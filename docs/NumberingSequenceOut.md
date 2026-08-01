# NumberingSequenceOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**document_type** | **str** |  | 
**prefix** | **str** |  | 
**date_pattern** | **str** |  | 
**padding** | **int** |  | 
**next_number** | **int** |  | 
**reset** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.numbering_sequence_out import NumberingSequenceOut

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingSequenceOut from a JSON string
numbering_sequence_out_instance = NumberingSequenceOut.from_json(json)
# print the JSON string representation of the object
print(NumberingSequenceOut.to_json())

# convert the object into a dict
numbering_sequence_out_dict = numbering_sequence_out_instance.to_dict()
# create an instance of NumberingSequenceOut from a dict
numbering_sequence_out_from_dict = NumberingSequenceOut.from_dict(numbering_sequence_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


