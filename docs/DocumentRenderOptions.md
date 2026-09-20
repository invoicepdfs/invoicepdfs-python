# DocumentRenderOptions

Render options for a document that is already stored.  For ``POST /documents/{id}/renders``. The stateless ``POST /documents/render`` takes the whole document inline instead.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**template_version** | **int** |  | [optional] 
**page_size** | **str** |  | [optional] [default to 'LETTER']
**expires_in** | **int** | How long the render stays downloadable, in seconds (1 minute to 7 days). It is also the lifetime of the signature in &#x60;download_url&#x60;, which is why it is bounded: an unbounded value meant an unbounded grant. A value below the floor used to be accepted and produced a render that had already expired. | [optional] [default to 3600]
**format** | **str** | &#x60;facturx_pdf&#x60; embeds the EN 16931 CII XML in a PDF/A-3, which is what a French or German counterparty means by Factur-X or ZUGFeRD. | [optional] [default to 'pdf']

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


