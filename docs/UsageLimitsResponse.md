# UsageLimitsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**UsageLimitsData**](UsageLimitsData.md) |  | 

## Example

```python
from invoicepdfs.models.usage_limits_response import UsageLimitsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UsageLimitsResponse from a JSON string
usage_limits_response_instance = UsageLimitsResponse.from_json(json)
# print the JSON string representation of the object
print(UsageLimitsResponse.to_json())

# convert the object into a dict
usage_limits_response_dict = usage_limits_response_instance.to_dict()
# create an instance of UsageLimitsResponse from a dict
usage_limits_response_from_dict = UsageLimitsResponse.from_dict(usage_limits_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


