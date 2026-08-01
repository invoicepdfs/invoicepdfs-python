# WorkspaceMembersListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WorkspaceMemberOut]**](WorkspaceMemberOut.md) |  | 

## Example

```python
from invoicepdfs.models.workspace_members_list_response import WorkspaceMembersListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WorkspaceMembersListResponse from a JSON string
workspace_members_list_response_instance = WorkspaceMembersListResponse.from_json(json)
# print the JSON string representation of the object
print(WorkspaceMembersListResponse.to_json())

# convert the object into a dict
workspace_members_list_response_dict = workspace_members_list_response_instance.to_dict()
# create an instance of WorkspaceMembersListResponse from a dict
workspace_members_list_response_from_dict = WorkspaceMembersListResponse.from_dict(workspace_members_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


