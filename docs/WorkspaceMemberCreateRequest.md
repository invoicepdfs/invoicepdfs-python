# WorkspaceMemberCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**role** | **str** |  | [optional] [default to 'member']

## Example

```python
from invoicepdfs.models.workspace_member_create_request import WorkspaceMemberCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WorkspaceMemberCreateRequest from a JSON string
workspace_member_create_request_instance = WorkspaceMemberCreateRequest.from_json(json)
# print the JSON string representation of the object
print(WorkspaceMemberCreateRequest.to_json())

# convert the object into a dict
workspace_member_create_request_dict = workspace_member_create_request_instance.to_dict()
# create an instance of WorkspaceMemberCreateRequest from a dict
workspace_member_create_request_from_dict = WorkspaceMemberCreateRequest.from_dict(workspace_member_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


