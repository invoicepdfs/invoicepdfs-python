# DocumentTypeOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**number_prefix** | **str** |  | 
**payable** | **bool** |  | 
**requires_source_document** | **bool** |  | 
**supports_reason** | **bool** |  | 
**line_item_type** | **str** |  | 
**actions** | **List[str]** |  | 

## Example

```python
from invoicepdfs.models.document_type_out import DocumentTypeOut

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentTypeOut from a JSON string
document_type_out_instance = DocumentTypeOut.from_json(json)
# print the JSON string representation of the object
print(DocumentTypeOut.to_json())

# convert the object into a dict
document_type_out_dict = document_type_out_instance.to_dict()
# create an instance of DocumentTypeOut from a dict
document_type_out_from_dict = DocumentTypeOut.from_dict(document_type_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


