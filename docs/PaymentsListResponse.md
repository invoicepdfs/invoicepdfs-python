# PaymentsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PaymentOut]**](PaymentOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.payments_list_response import PaymentsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentsListResponse from a JSON string
payments_list_response_instance = PaymentsListResponse.from_json(json)
# print the JSON string representation of the object
print(PaymentsListResponse.to_json())

# convert the object into a dict
payments_list_response_dict = payments_list_response_instance.to_dict()
# create an instance of PaymentsListResponse from a dict
payments_list_response_from_dict = PaymentsListResponse.from_dict(payments_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


