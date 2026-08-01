# RecurringInvoicesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[RecurringInvoiceOut]**](RecurringInvoiceOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | 

## Example

```python
from invoicepdfs.models.recurring_invoices_list_response import RecurringInvoicesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringInvoicesListResponse from a JSON string
recurring_invoices_list_response_instance = RecurringInvoicesListResponse.from_json(json)
# print the JSON string representation of the object
print(RecurringInvoicesListResponse.to_json())

# convert the object into a dict
recurring_invoices_list_response_dict = recurring_invoices_list_response_instance.to_dict()
# create an instance of RecurringInvoicesListResponse from a dict
recurring_invoices_list_response_from_dict = RecurringInvoicesListResponse.from_dict(recurring_invoices_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


