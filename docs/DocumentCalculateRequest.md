# DocumentCalculateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 

## Example

```python
from invoicepdfs.models.document_calculate_request import DocumentCalculateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentCalculateRequest from a JSON string
document_calculate_request_instance = DocumentCalculateRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentCalculateRequest.to_json())

# convert the object into a dict
document_calculate_request_dict = document_calculate_request_instance.to_dict()
# create an instance of DocumentCalculateRequest from a dict
document_calculate_request_from_dict = DocumentCalculateRequest.from_dict(document_calculate_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


