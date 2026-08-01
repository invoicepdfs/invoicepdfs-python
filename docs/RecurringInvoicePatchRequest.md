# RecurringInvoicePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**frequency** | **str** |  | [optional] 
**interval** | **int** |  | [optional] 
**end_date** | **date** |  | [optional] 
**max_occurrences** | **int** |  | [optional] 
**numbering_sequence_id** | **str** |  | [optional] 
**auto_finalize** | **bool** |  | [optional] 
**invoice_template** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.recurring_invoice_patch_request import RecurringInvoicePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringInvoicePatchRequest from a JSON string
recurring_invoice_patch_request_instance = RecurringInvoicePatchRequest.from_json(json)
# print the JSON string representation of the object
print(RecurringInvoicePatchRequest.to_json())

# convert the object into a dict
recurring_invoice_patch_request_dict = recurring_invoice_patch_request_instance.to_dict()
# create an instance of RecurringInvoicePatchRequest from a dict
recurring_invoice_patch_request_from_dict = RecurringInvoicePatchRequest.from_dict(recurring_invoice_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


