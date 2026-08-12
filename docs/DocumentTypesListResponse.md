# DocumentTypesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DocumentTypeOut]**](DocumentTypeOut.md) |  | 

## Example

```python
from invoicepdfs.models.document_types_list_response import DocumentTypesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentTypesListResponse from a JSON string
document_types_list_response_instance = DocumentTypesListResponse.from_json(json)
# print the JSON string representation of the object
print(DocumentTypesListResponse.to_json())

# convert the object into a dict
document_types_list_response_dict = document_types_list_response_instance.to_dict()
# create an instance of DocumentTypesListResponse from a dict
document_types_list_response_from_dict = DocumentTypesListResponse.from_dict(document_types_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


