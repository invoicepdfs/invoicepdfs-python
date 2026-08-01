# DocumentInvoiceDataInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_number** | **str** |  | 
**issue_date** | **date** |  | 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | 
**seller** | [**DocumentPartyInput**](DocumentPartyInput.md) |  | 
**buyer** | [**DocumentPartyInput**](DocumentPartyInput.md) |  | 
**ship_to** | [**DocumentPartyInput**](DocumentPartyInput.md) |  | [optional] 
**line_items** | [**List[DocumentLineItemInput]**](DocumentLineItemInput.md) |  | 
**discounts** | [**List[DocumentDiscountInput]**](DocumentDiscountInput.md) |  | [optional] 
**shipping** | [**DocumentShippingInput**](DocumentShippingInput.md) |  | [optional] 
**custom_fields** | [**List[DocumentCustomFieldInput]**](DocumentCustomFieldInput.md) |  | [optional] 
**payment** | [**DocumentPaymentInput**](DocumentPaymentInput.md) |  | [optional] 
**branding** | [**DocumentBrandingInput**](DocumentBrandingInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_invoice_data_input import DocumentInvoiceDataInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentInvoiceDataInput from a JSON string
document_invoice_data_input_instance = DocumentInvoiceDataInput.from_json(json)
# print the JSON string representation of the object
print(DocumentInvoiceDataInput.to_json())

# convert the object into a dict
document_invoice_data_input_dict = document_invoice_data_input_instance.to_dict()
# create an instance of DocumentInvoiceDataInput from a dict
document_invoice_data_input_from_dict = DocumentInvoiceDataInput.from_dict(document_invoice_data_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


