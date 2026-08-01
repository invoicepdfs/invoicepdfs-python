# AuditEventOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**actor** | **str** |  | 
**action** | **str** |  | 
**resource_type** | **str** |  | 
**resource_id** | **str** |  | 
**workspace_id** | **str** |  | [optional] 
**ip_address** | **str** |  | [optional] 
**user_agent** | **str** |  | [optional] 
**request_id** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.audit_event_out import AuditEventOut

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEventOut from a JSON string
audit_event_out_instance = AuditEventOut.from_json(json)
# print the JSON string representation of the object
print(AuditEventOut.to_json())

# convert the object into a dict
audit_event_out_dict = audit_event_out_instance.to_dict()
# create an instance of AuditEventOut from a dict
audit_event_out_from_dict = AuditEventOut.from_dict(audit_event_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


