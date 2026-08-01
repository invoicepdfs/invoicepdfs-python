# InvoicesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InvoiceOut]**](InvoiceOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.invoices_list_response import InvoicesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvoicesListResponse from a JSON string
invoices_list_response_instance = InvoicesListResponse.from_json(json)
# print the JSON string representation of the object
print(InvoicesListResponse.to_json())

# convert the object into a dict
invoices_list_response_dict = invoices_list_response_instance.to_dict()
# create an instance of InvoicesListResponse from a dict
invoices_list_response_from_dict = InvoicesListResponse.from_dict(invoices_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


