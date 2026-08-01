# InvoiceDraftRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_number** | **str** |  | 
**document_type** | **str** |  | [optional] [default to 'invoice']
**issue_date** | **date** |  | 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**ship_to** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**line_items** | [**List[InvoiceLineItemInput]**](InvoiceLineItemInput.md) |  | 
**discounts** | [**List[InvoiceDiscountInput]**](InvoiceDiscountInput.md) |  | [optional] 
**shipping** | [**InvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**notes** | [**List[InvoiceNoteInput]**](InvoiceNoteInput.md) |  | [optional] 
**terms** | [**List[InvoiceTermInput]**](InvoiceTermInput.md) |  | [optional] 
**custom_fields** | [**List[InvoiceCustomFieldInput]**](InvoiceCustomFieldInput.md) |  | [optional] 
**payment** | [**InvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**branding** | [**InvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_draft_request import InvoiceDraftRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceDraftRequest from a JSON string
invoice_draft_request_instance = InvoiceDraftRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceDraftRequest.to_json())

# convert the object into a dict
invoice_draft_request_dict = invoice_draft_request_instance.to_dict()
# create an instance of InvoiceDraftRequest from a dict
invoice_draft_request_from_dict = InvoiceDraftRequest.from_dict(invoice_draft_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


