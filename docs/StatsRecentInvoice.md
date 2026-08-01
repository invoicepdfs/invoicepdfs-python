# StatsRecentInvoice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**invoice_number** | **str** |  | 
**document_type** | **str** |  | 
**status** | **str** |  | 
**currency** | **str** |  | 
**total_amount** | **str** |  | 
**issue_date** | **str** |  | 

## Example

```python
from invoicepdfs.models.stats_recent_invoice import StatsRecentInvoice

# TODO update the JSON string below
json = "{}"
# create an instance of StatsRecentInvoice from a JSON string
stats_recent_invoice_instance = StatsRecentInvoice.from_json(json)
# print the JSON string representation of the object
print(StatsRecentInvoice.to_json())

# convert the object into a dict
stats_recent_invoice_dict = stats_recent_invoice_instance.to_dict()
# create an instance of StatsRecentInvoice from a dict
stats_recent_invoice_from_dict = StatsRecentInvoice.from_dict(stats_recent_invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


