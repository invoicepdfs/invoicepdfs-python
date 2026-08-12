# TimezonesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TimezoneOut]**](TimezoneOut.md) |  | 

## Example

```python
from invoicepdfs.models.timezones_list_response import TimezonesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TimezonesListResponse from a JSON string
timezones_list_response_instance = TimezonesListResponse.from_json(json)
# print the JSON string representation of the object
print(TimezonesListResponse.to_json())

# convert the object into a dict
timezones_list_response_dict = timezones_list_response_instance.to_dict()
# create an instance of TimezonesListResponse from a dict
timezones_list_response_from_dict = TimezonesListResponse.from_dict(timezones_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


