# RecurringInvoiceOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**frequency** | **str** |  | 
**interval** | **int** |  | 
**next_occurrence_date** | **date** |  | 
**end_date** | **date** |  | 
**occurrences_created** | **int** |  | 
**max_occurrences** | **int** |  | 
**numbering_sequence_id** | **str** |  | 
**auto_finalize** | **bool** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.recurring_invoice_out import RecurringInvoiceOut

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringInvoiceOut from a JSON string
recurring_invoice_out_instance = RecurringInvoiceOut.from_json(json)
# print the JSON string representation of the object
print(RecurringInvoiceOut.to_json())

# convert the object into a dict
recurring_invoice_out_dict = recurring_invoice_out_instance.to_dict()
# create an instance of RecurringInvoiceOut from a dict
recurring_invoice_out_from_dict = RecurringInvoiceOut.from_dict(recurring_invoice_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


