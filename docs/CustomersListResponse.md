# CustomersListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomerOut]**](CustomerOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.customers_list_response import CustomersListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomersListResponse from a JSON string
customers_list_response_instance = CustomersListResponse.from_json(json)
# print the JSON string representation of the object
print(CustomersListResponse.to_json())

# convert the object into a dict
customers_list_response_dict = customers_list_response_instance.to_dict()
# create an instance of CustomersListResponse from a dict
customers_list_response_from_dict = CustomersListResponse.from_dict(customers_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


