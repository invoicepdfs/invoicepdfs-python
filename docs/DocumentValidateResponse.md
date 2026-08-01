# DocumentValidateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | **Dict[str, bool]** |  | 

## Example

```python
from invoicepdfs.models.document_validate_response import DocumentValidateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentValidateResponse from a JSON string
document_validate_response_instance = DocumentValidateResponse.from_json(json)
# print the JSON string representation of the object
print(DocumentValidateResponse.to_json())

# convert the object into a dict
document_validate_response_dict = document_validate_response_instance.to_dict()
# create an instance of DocumentValidateResponse from a dict
document_validate_response_from_dict = DocumentValidateResponse.from_dict(document_validate_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


