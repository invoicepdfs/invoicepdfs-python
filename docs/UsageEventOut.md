# UsageEventOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**render_id** | **str** |  | 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.usage_event_out import UsageEventOut

# TODO update the JSON string below
json = "{}"
# create an instance of UsageEventOut from a JSON string
usage_event_out_instance = UsageEventOut.from_json(json)
# print the JSON string representation of the object
print(UsageEventOut.to_json())

# convert the object into a dict
usage_event_out_dict = usage_event_out_instance.to_dict()
# create an instance of UsageEventOut from a dict
usage_event_out_from_dict = UsageEventOut.from_dict(usage_event_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


