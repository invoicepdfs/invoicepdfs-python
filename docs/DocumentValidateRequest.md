# DocumentValidateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 

## Example

```python
from invoicepdfs.models.document_validate_request import DocumentValidateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentValidateRequest from a JSON string
document_validate_request_instance = DocumentValidateRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentValidateRequest.to_json())

# convert the object into a dict
document_validate_request_dict = document_validate_request_instance.to_dict()
# create an instance of DocumentValidateRequest from a dict
document_validate_request_from_dict = DocumentValidateRequest.from_dict(document_validate_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


