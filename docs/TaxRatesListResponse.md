# TaxRatesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TaxRateOut]**](TaxRateOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.tax_rates_list_response import TaxRatesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRatesListResponse from a JSON string
tax_rates_list_response_instance = TaxRatesListResponse.from_json(json)
# print the JSON string representation of the object
print(TaxRatesListResponse.to_json())

# convert the object into a dict
tax_rates_list_response_dict = tax_rates_list_response_instance.to_dict()
# create an instance of TaxRatesListResponse from a dict
tax_rates_list_response_from_dict = TaxRatesListResponse.from_dict(tax_rates_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


