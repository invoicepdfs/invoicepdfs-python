# CurrenciesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CurrencyOut]**](CurrencyOut.md) |  | 

## Example

```python
from invoicepdfs.models.currencies_list_response import CurrenciesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CurrenciesListResponse from a JSON string
currencies_list_response_instance = CurrenciesListResponse.from_json(json)
# print the JSON string representation of the object
print(CurrenciesListResponse.to_json())

# convert the object into a dict
currencies_list_response_dict = currencies_list_response_instance.to_dict()
# create an instance of CurrenciesListResponse from a dict
currencies_list_response_from_dict = CurrenciesListResponse.from_dict(currencies_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


