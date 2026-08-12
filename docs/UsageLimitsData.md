# UsageLimitsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**renders** | [**UsageRenderLimits**](UsageRenderLimits.md) |  | 
**rate_limit** | [**UsageRateLimit**](UsageRateLimit.md) |  | 

## Example

```python
from invoicepdfs.models.usage_limits_data import UsageLimitsData

# TODO update the JSON string below
json = "{}"
# create an instance of UsageLimitsData from a JSON string
usage_limits_data_instance = UsageLimitsData.from_json(json)
# print the JSON string representation of the object
print(UsageLimitsData.to_json())

# convert the object into a dict
usage_limits_data_dict = usage_limits_data_instance.to_dict()
# create an instance of UsageLimitsData from a dict
usage_limits_data_from_dict = UsageLimitsData.from_dict(usage_limits_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


