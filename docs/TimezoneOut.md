# TimezoneOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**offset** | **str** |  | 

## Example

```python
from invoicepdfs.models.timezone_out import TimezoneOut

# TODO update the JSON string below
json = "{}"
# create an instance of TimezoneOut from a JSON string
timezone_out_instance = TimezoneOut.from_json(json)
# print the JSON string representation of the object
print(TimezoneOut.to_json())

# convert the object into a dict
timezone_out_dict = timezone_out_instance.to_dict()
# create an instance of TimezoneOut from a dict
timezone_out_from_dict = TimezoneOut.from_dict(timezone_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


