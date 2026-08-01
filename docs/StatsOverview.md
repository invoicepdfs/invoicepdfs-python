# StatsOverview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**counts** | [**StatsCounts**](StatsCounts.md) |  | 
**invoice_status_counts** | **Dict[str, int]** |  | 
**recent_invoices** | [**List[StatsRecentInvoice]**](StatsRecentInvoice.md) |  | 

## Example

```python
from invoicepdfs.models.stats_overview import StatsOverview

# TODO update the JSON string below
json = "{}"
# create an instance of StatsOverview from a JSON string
stats_overview_instance = StatsOverview.from_json(json)
# print the JSON string representation of the object
print(StatsOverview.to_json())

# convert the object into a dict
stats_overview_dict = stats_overview_instance.to_dict()
# create an instance of StatsOverview from a dict
stats_overview_from_dict = StatsOverview.from_dict(stats_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


