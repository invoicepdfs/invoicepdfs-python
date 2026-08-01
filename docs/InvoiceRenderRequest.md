# InvoiceRenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**page_size** | **str** |  | [optional] [default to 'LETTER']
**expires_in** | **int** |  | [optional] [default to 3600]

## Example

```python
from invoicepdfs.models.invoice_render_request import InvoiceRenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceRenderRequest from a JSON string
invoice_render_request_instance = InvoiceRenderRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceRenderRequest.to_json())

# convert the object into a dict
invoice_render_request_dict = invoice_render_request_instance.to_dict()
# create an instance of InvoiceRenderRequest from a dict
invoice_render_request_from_dict = InvoiceRenderRequest.from_dict(invoice_render_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


