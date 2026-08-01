# InvoiceAttachmentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InvoiceAttachmentOut**](InvoiceAttachmentOut.md) |  | 

## Example

```python
from invoicepdfs.models.invoice_attachment_response import InvoiceAttachmentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceAttachmentResponse from a JSON string
invoice_attachment_response_instance = InvoiceAttachmentResponse.from_json(json)
# print the JSON string representation of the object
print(InvoiceAttachmentResponse.to_json())

# convert the object into a dict
invoice_attachment_response_dict = invoice_attachment_response_instance.to_dict()
# create an instance of InvoiceAttachmentResponse from a dict
invoice_attachment_response_from_dict = InvoiceAttachmentResponse.from_dict(invoice_attachment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


