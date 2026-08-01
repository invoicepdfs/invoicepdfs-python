# DocumentRenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 
**template** | [**DocumentTemplateRef**](DocumentTemplateRef.md) |  | 
**output** | [**DocumentOutputOptions**](DocumentOutputOptions.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_render_request import DocumentRenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentRenderRequest from a JSON string
document_render_request_instance = DocumentRenderRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentRenderRequest.to_json())

# convert the object into a dict
document_render_request_dict = document_render_request_instance.to_dict()
# create an instance of DocumentRenderRequest from a dict
document_render_request_from_dict = DocumentRenderRequest.from_dict(document_render_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


