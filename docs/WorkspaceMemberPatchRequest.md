# WorkspaceMemberPatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.workspace_member_patch_request import WorkspaceMemberPatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WorkspaceMemberPatchRequest from a JSON string
workspace_member_patch_request_instance = WorkspaceMemberPatchRequest.from_json(json)
# print the JSON string representation of the object
print(WorkspaceMemberPatchRequest.to_json())

# convert the object into a dict
workspace_member_patch_request_dict = workspace_member_patch_request_instance.to_dict()
# create an instance of WorkspaceMemberPatchRequest from a dict
workspace_member_patch_request_from_dict = WorkspaceMemberPatchRequest.from_dict(workspace_member_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


