# NumberingSequenceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**NumberingSequenceOut**](NumberingSequenceOut.md) |  | 

## Example

```python
from invoicepdfs.models.numbering_sequence_response import NumberingSequenceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingSequenceResponse from a JSON string
numbering_sequence_response_instance = NumberingSequenceResponse.from_json(json)
# print the JSON string representation of the object
print(NumberingSequenceResponse.to_json())

# convert the object into a dict
numbering_sequence_response_dict = numbering_sequence_response_instance.to_dict()
# create an instance of NumberingSequenceResponse from a dict
numbering_sequence_response_from_dict = NumberingSequenceResponse.from_dict(numbering_sequence_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


