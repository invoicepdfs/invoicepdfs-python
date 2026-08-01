# SimpleBoolResponse

Generic boolean response envelope.  Example: {\"data\": {\"deleted\": true}}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | **Dict[str, bool]** |  | 

## Example

```python
from invoicepdfs.models.simple_bool_response import SimpleBoolResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SimpleBoolResponse from a JSON string
simple_bool_response_instance = SimpleBoolResponse.from_json(json)
# print the JSON string representation of the object
print(SimpleBoolResponse.to_json())

# convert the object into a dict
simple_bool_response_dict = simple_bool_response_instance.to_dict()
# create an instance of SimpleBoolResponse from a dict
simple_bool_response_from_dict = SimpleBoolResponse.from_dict(simple_bool_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


