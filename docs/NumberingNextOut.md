# NumberingNextOut

What POST /numbering-sequences/{id}/next allocated.  The number is the point of the call. It used to answer with the sequence row instead, so a caller burned a number and had to reconstruct the string itself from prefix, date pattern and padding — the one thing the endpoint exists to do for them.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **str** |  | 
**sequence_id** | **str** |  | 
**next_number** | **int** | The counter after this allocation | 

## Example

```python
from invoicepdfs.models.numbering_next_out import NumberingNextOut

# TODO update the JSON string below
json = "{}"
# create an instance of NumberingNextOut from a JSON string
numbering_next_out_instance = NumberingNextOut.from_json(json)
# print the JSON string representation of the object
print(NumberingNextOut.to_json())

# convert the object into a dict
numbering_next_out_dict = numbering_next_out_instance.to_dict()
# create an instance of NumberingNextOut from a dict
numbering_next_out_from_dict = NumberingNextOut.from_dict(numbering_next_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


