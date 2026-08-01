# InvoiceOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**invoice_number** | **str** |  | 
**document_type** | **str** |  | 
**issue_date** | **date** |  | 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**invoice** | **Dict[str, object]** |  | 
**totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**finalized_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_out import InvoiceOut

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceOut from a JSON string
invoice_out_instance = InvoiceOut.from_json(json)
# print the JSON string representation of the object
print(InvoiceOut.to_json())

# convert the object into a dict
invoice_out_dict = invoice_out_instance.to_dict()
# create an instance of InvoiceOut from a dict
invoice_out_from_dict = InvoiceOut.from_dict(invoice_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


