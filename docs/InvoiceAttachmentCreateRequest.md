# InvoiceAttachmentCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_id** | **str** |  | 
**label** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_attachment_create_request import InvoiceAttachmentCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceAttachmentCreateRequest from a JSON string
invoice_attachment_create_request_instance = InvoiceAttachmentCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceAttachmentCreateRequest.to_json())

# convert the object into a dict
invoice_attachment_create_request_dict = invoice_attachment_create_request_instance.to_dict()
# create an instance of InvoiceAttachmentCreateRequest from a dict
invoice_attachment_create_request_from_dict = InvoiceAttachmentCreateRequest.from_dict(invoice_attachment_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


