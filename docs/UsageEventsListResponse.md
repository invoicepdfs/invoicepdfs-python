# UsageEventsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[UsageEventOut]**](UsageEventOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.usage_events_list_response import UsageEventsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UsageEventsListResponse from a JSON string
usage_events_list_response_instance = UsageEventsListResponse.from_json(json)
# print the JSON string representation of the object
print(UsageEventsListResponse.to_json())

# convert the object into a dict
usage_events_list_response_dict = usage_events_list_response_instance.to_dict()
# create an instance of UsageEventsListResponse from a dict
usage_events_list_response_from_dict = UsageEventsListResponse.from_dict(usage_events_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


