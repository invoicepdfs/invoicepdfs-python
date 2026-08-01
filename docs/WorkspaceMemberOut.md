# WorkspaceMemberOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**workspace_id** | **str** |  | 
**email** | **str** |  | 
**role** | **str** |  | 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.workspace_member_out import WorkspaceMemberOut

# TODO update the JSON string below
json = "{}"
# create an instance of WorkspaceMemberOut from a JSON string
workspace_member_out_instance = WorkspaceMemberOut.from_json(json)
# print the JSON string representation of the object
print(WorkspaceMemberOut.to_json())

# convert the object into a dict
workspace_member_out_dict = workspace_member_out_instance.to_dict()
# create an instance of WorkspaceMemberOut from a dict
workspace_member_out_from_dict = WorkspaceMemberOut.from_dict(workspace_member_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


