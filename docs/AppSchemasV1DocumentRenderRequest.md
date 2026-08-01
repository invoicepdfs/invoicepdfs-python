# AppSchemasV1DocumentRenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 
**template** | [**DocumentTemplateRef**](DocumentTemplateRef.md) |  | 
**output** | [**DocumentOutputOptions**](DocumentOutputOptions.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.app_schemas_v1_document_render_request import AppSchemasV1DocumentRenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppSchemasV1DocumentRenderRequest from a JSON string
app_schemas_v1_document_render_request_instance = AppSchemasV1DocumentRenderRequest.from_json(json)
# print the JSON string representation of the object
print(AppSchemasV1DocumentRenderRequest.to_json())

# convert the object into a dict
app_schemas_v1_document_render_request_dict = app_schemas_v1_document_render_request_instance.to_dict()
# create an instance of AppSchemasV1DocumentRenderRequest from a dict
app_schemas_v1_document_render_request_from_dict = AppSchemasV1DocumentRenderRequest.from_dict(app_schemas_v1_document_render_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


