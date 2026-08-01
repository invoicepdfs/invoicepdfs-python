# DocumentCustomFieldInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from invoicepdfs.models.document_custom_field_input import DocumentCustomFieldInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentCustomFieldInput from a JSON string
document_custom_field_input_instance = DocumentCustomFieldInput.from_json(json)
# print the JSON string representation of the object
print(DocumentCustomFieldInput.to_json())

# convert the object into a dict
document_custom_field_input_dict = document_custom_field_input_instance.to_dict()
# create an instance of DocumentCustomFieldInput from a dict
document_custom_field_input_from_dict = DocumentCustomFieldInput.from_dict(document_custom_field_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


