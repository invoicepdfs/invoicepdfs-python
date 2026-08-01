# StatsCounts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoices** | **int** |  | 
**customers** | **int** |  | 
**business_profiles** | **int** |  | 

## Example

```python
from invoicepdfs.models.stats_counts import StatsCounts

# TODO update the JSON string below
json = "{}"
# create an instance of StatsCounts from a JSON string
stats_counts_instance = StatsCounts.from_json(json)
# print the JSON string representation of the object
print(StatsCounts.to_json())

# convert the object into a dict
stats_counts_dict = stats_counts_instance.to_dict()
# create an instance of StatsCounts from a dict
stats_counts_from_dict = StatsCounts.from_dict(stats_counts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


