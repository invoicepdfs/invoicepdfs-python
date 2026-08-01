# DocumentsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DocumentOut]**](DocumentOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.documents_list_response import DocumentsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentsListResponse from a JSON string
documents_list_response_instance = DocumentsListResponse.from_json(json)
# print the JSON string representation of the object
print(DocumentsListResponse.to_json())

# convert the object into a dict
documents_list_response_dict = documents_list_response_instance.to_dict()
# create an instance of DocumentsListResponse from a dict
documents_list_response_from_dict = DocumentsListResponse.from_dict(documents_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


