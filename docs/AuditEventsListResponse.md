# AuditEventsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AuditEventOut]**](AuditEventOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.audit_events_list_response import AuditEventsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEventsListResponse from a JSON string
audit_events_list_response_instance = AuditEventsListResponse.from_json(json)
# print the JSON string representation of the object
print(AuditEventsListResponse.to_json())

# convert the object into a dict
audit_events_list_response_dict = audit_events_list_response_instance.to_dict()
# create an instance of AuditEventsListResponse from a dict
audit_events_list_response_from_dict = AuditEventsListResponse.from_dict(audit_events_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


