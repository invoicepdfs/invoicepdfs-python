# InvoiceCreateRequest


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
from invoicepdfs.models.invoice_create_request import InvoiceCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceCreateRequest from a JSON string
invoice_create_request_instance = InvoiceCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceCreateRequest.to_json())

# convert the object into a dict
invoice_create_request_dict = invoice_create_request_instance.to_dict()
# create an instance of InvoiceCreateRequest from a dict
invoice_create_request_from_dict = InvoiceCreateRequest.from_dict(invoice_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


