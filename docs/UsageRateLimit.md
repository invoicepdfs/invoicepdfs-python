# UsageRateLimit


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**requests_per_second** | **int** |  | 

## Example

```python
from invoicepdfs.models.usage_rate_limit import UsageRateLimit

# TODO update the JSON string below
json = "{}"
# create an instance of UsageRateLimit from a JSON string
usage_rate_limit_instance = UsageRateLimit.from_json(json)
# print the JSON string representation of the object
print(UsageRateLimit.to_json())

# convert the object into a dict
usage_rate_limit_dict = usage_rate_limit_instance.to_dict()
# create an instance of UsageRateLimit from a dict
usage_rate_limit_from_dict = UsageRateLimit.from_dict(usage_rate_limit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


