# DocumentRenderOptions

Render options for an already-stored document (``POST /documents/{id}/renders``).  Distinct from ``app.schemas.v1.DocumentRenderRequest``, which carries a full inline document for the stateless ``POST /documents/render``. Two classes sharing one name made FastAPI fall back to module-qualified schema names in the spec (``app__documents__schemas__DocumentRenderRequest``), which the SDK generators turned into ``AppDocumentsSchemasDocumentRenderRequest``.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**page_size** | **str** |  | [optional] [default to 'LETTER']
**expires_in** | **int** |  | [optional] [default to 3600]

## Example

```python
from invoicepdfs.models.document_render_options import DocumentRenderOptions

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentRenderOptions from a JSON string
document_render_options_instance = DocumentRenderOptions.from_json(json)
# print the JSON string representation of the object
print(DocumentRenderOptions.to_json())

# convert the object into a dict
document_render_options_dict = document_render_options_instance.to_dict()
# create an instance of DocumentRenderOptions from a dict
document_render_options_from_dict = DocumentRenderOptions.from_dict(document_render_options_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


