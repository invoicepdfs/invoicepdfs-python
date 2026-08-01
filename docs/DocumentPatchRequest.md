# DocumentPatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **str** |  | [optional] 
**document_type** | **str** |  | [optional] 
**issue_date** | **date** |  | [optional] 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | [optional] 
**customer_id** | **str** |  | [optional] 
**source_document_id** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**ship_to** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**line_items** | [**List[StandardLineItemInput]**](StandardLineItemInput.md) |  | [optional] 
**discounts** | [**List[LineItemDiscountInput]**](LineItemDiscountInput.md) |  | [optional] 
**shipping** | [**InvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**notes** | [**List[InvoiceNoteInput]**](InvoiceNoteInput.md) |  | [optional] 
**terms** | [**List[InvoiceTermInput]**](InvoiceTermInput.md) |  | [optional] 
**custom_fields** | [**List[InvoiceCustomFieldInput]**](InvoiceCustomFieldInput.md) |  | [optional] 
**payment** | [**InvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**branding** | [**InvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_patch_request import DocumentPatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentPatchRequest from a JSON string
document_patch_request_instance = DocumentPatchRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentPatchRequest.to_json())

# convert the object into a dict
document_patch_request_dict = document_patch_request_instance.to_dict()
# create an instance of DocumentPatchRequest from a dict
document_patch_request_from_dict = DocumentPatchRequest.from_dict(document_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


