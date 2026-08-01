# InvoiceAttachmentsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InvoiceAttachmentOut]**](InvoiceAttachmentOut.md) |  | 

## Example

```python
from invoicepdfs.models.invoice_attachments_list_response import InvoiceAttachmentsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceAttachmentsListResponse from a JSON string
invoice_attachments_list_response_instance = InvoiceAttachmentsListResponse.from_json(json)
# print the JSON string representation of the object
print(InvoiceAttachmentsListResponse.to_json())

# convert the object into a dict
invoice_attachments_list_response_dict = invoice_attachments_list_response_instance.to_dict()
# create an instance of InvoiceAttachmentsListResponse from a dict
invoice_attachments_list_response_from_dict = InvoiceAttachmentsListResponse.from_dict(invoice_attachments_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


