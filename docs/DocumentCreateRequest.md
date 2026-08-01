# DocumentCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**number** | **str** |  | 
**issue_date** | **date** |  | 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**source_document_id** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**ship_to** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**line_items** | [**List[StandardLineItemInput]**](StandardLineItemInput.md) |  | 
**discounts** | [**List[LineItemDiscountInput]**](LineItemDiscountInput.md) |  | [optional] 
**shipping** | [**InvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**notes** | [**List[InvoiceNoteInput]**](InvoiceNoteInput.md) |  | [optional] 
**terms** | [**List[InvoiceTermInput]**](InvoiceTermInput.md) |  | [optional] 
**custom_fields** | [**List[InvoiceCustomFieldInput]**](InvoiceCustomFieldInput.md) |  | [optional] 
**payment** | [**InvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**branding** | [**InvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_create_request import DocumentCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentCreateRequest from a JSON string
document_create_request_instance = DocumentCreateRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentCreateRequest.to_json())

# convert the object into a dict
document_create_request_dict = document_create_request_instance.to_dict()
# create an instance of DocumentCreateRequest from a dict
document_create_request_from_dict = DocumentCreateRequest.from_dict(document_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


