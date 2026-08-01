# InvoiceAttachmentOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**invoice_id** | **str** |  | 
**file_id** | **str** |  | 
**label** | **str** |  | [optional] 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.invoice_attachment_out import InvoiceAttachmentOut

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceAttachmentOut from a JSON string
invoice_attachment_out_instance = InvoiceAttachmentOut.from_json(json)
# print the JSON string representation of the object
print(InvoiceAttachmentOut.to_json())

# convert the object into a dict
invoice_attachment_out_dict = invoice_attachment_out_instance.to_dict()
# create an instance of InvoiceAttachmentOut from a dict
invoice_attachment_out_from_dict = InvoiceAttachmentOut.from_dict(invoice_attachment_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


