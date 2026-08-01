# InvoicePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_number** | **str** |  | [optional] 
**document_type** | **str** |  | [optional] 
**issue_date** | **date** |  | [optional] 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | [optional] 
**customer_id** | **str** |  | [optional] 
**ship_to** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**line_items** | [**List[InvoiceLineItemInput]**](InvoiceLineItemInput.md) |  | [optional] 
**discounts** | [**List[InvoiceDiscountInput]**](InvoiceDiscountInput.md) |  | [optional] 
**shipping** | [**InvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**notes** | [**List[InvoiceNoteInput]**](InvoiceNoteInput.md) |  | [optional] 
**terms** | [**List[InvoiceTermInput]**](InvoiceTermInput.md) |  | [optional] 
**custom_fields** | [**List[InvoiceCustomFieldInput]**](InvoiceCustomFieldInput.md) |  | [optional] 
**payment** | [**InvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**branding** | [**InvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_patch_request import InvoicePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoicePatchRequest from a JSON string
invoice_patch_request_instance = InvoicePatchRequest.from_json(json)
# print the JSON string representation of the object
print(InvoicePatchRequest.to_json())

# convert the object into a dict
invoice_patch_request_dict = invoice_patch_request_instance.to_dict()
# create an instance of InvoicePatchRequest from a dict
invoice_patch_request_from_dict = InvoicePatchRequest.from_dict(invoice_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


