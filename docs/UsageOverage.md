# UsageOverage

Renders past the quota this period, and what they cost.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] [default to False]
**available** | **bool** |  | [optional] [default to False]
**renders** | **int** |  | [optional] [default to 0]
**price_millicents** | **int** |  | [optional] 
**estimated_cost_cents** | **int** |  | [optional] [default to 0]

## Example

```python
from invoicepdfs.models.usage_overage import UsageOverage

# TODO update the JSON string below
json = "{}"
# create an instance of UsageOverage from a JSON string
usage_overage_instance = UsageOverage.from_json(json)
# print the JSON string representation of the object
print(UsageOverage.to_json())

# convert the object into a dict
usage_overage_dict = usage_overage_instance.to_dict()
# create an instance of UsageOverage from a dict
usage_overage_from_dict = UsageOverage.from_dict(usage_overage_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


