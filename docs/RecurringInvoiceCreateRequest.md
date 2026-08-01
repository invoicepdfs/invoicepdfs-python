# RecurringInvoiceCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**frequency** | **str** | daily, weekly, monthly, quarterly, or yearly | 
**interval** | **int** | Every N periods | [optional] [default to 1]
**start_date** | **date** | Date of the first invoice | 
**end_date** | **date** |  | [optional] 
**max_occurrences** | **int** |  | [optional] 
**numbering_sequence_id** | **str** |  | [optional] 
**auto_finalize** | **bool** | Automatically finalize generated invoices | [optional] [default to False]
**invoice_template** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | 

## Example

```python
from invoicepdfs.models.recurring_invoice_create_request import RecurringInvoiceCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringInvoiceCreateRequest from a JSON string
recurring_invoice_create_request_instance = RecurringInvoiceCreateRequest.from_json(json)
# print the JSON string representation of the object
print(RecurringInvoiceCreateRequest.to_json())

# convert the object into a dict
recurring_invoice_create_request_dict = recurring_invoice_create_request_instance.to_dict()
# create an instance of RecurringInvoiceCreateRequest from a dict
recurring_invoice_create_request_from_dict = RecurringInvoiceCreateRequest.from_dict(recurring_invoice_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


