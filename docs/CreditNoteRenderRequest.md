# CreditNoteRenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**page_size** | **str** |  | [optional] [default to 'LETTER']

## Example

```python
from invoicepdfs.models.credit_note_render_request import CreditNoteRenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreditNoteRenderRequest from a JSON string
credit_note_render_request_instance = CreditNoteRenderRequest.from_json(json)
# print the JSON string representation of the object
print(CreditNoteRenderRequest.to_json())

# convert the object into a dict
credit_note_render_request_dict = credit_note_render_request_instance.to_dict()
# create an instance of CreditNoteRenderRequest from a dict
credit_note_render_request_from_dict = CreditNoteRenderRequest.from_dict(credit_note_render_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


