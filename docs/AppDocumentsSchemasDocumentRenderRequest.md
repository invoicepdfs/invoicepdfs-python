# AppDocumentsSchemasDocumentRenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**page_size** | **str** |  | [optional] [default to 'LETTER']
**expires_in** | **int** |  | [optional] [default to 3600]

## Example

```python
from invoicepdfs.models.app_documents_schemas_document_render_request import AppDocumentsSchemasDocumentRenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppDocumentsSchemasDocumentRenderRequest from a JSON string
app_documents_schemas_document_render_request_instance = AppDocumentsSchemasDocumentRenderRequest.from_json(json)
# print the JSON string representation of the object
print(AppDocumentsSchemasDocumentRenderRequest.to_json())

# convert the object into a dict
app_documents_schemas_document_render_request_dict = app_documents_schemas_document_render_request_instance.to_dict()
# create an instance of AppDocumentsSchemasDocumentRenderRequest from a dict
app_documents_schemas_document_render_request_from_dict = AppDocumentsSchemasDocumentRenderRequest.from_dict(app_documents_schemas_document_render_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


