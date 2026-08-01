# TaxRateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TaxRateOut**](TaxRateOut.md) |  | 

## Example

```python
from invoicepdfs.models.tax_rate_response import TaxRateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRateResponse from a JSON string
tax_rate_response_instance = TaxRateResponse.from_json(json)
# print the JSON string representation of the object
print(TaxRateResponse.to_json())

# convert the object into a dict
tax_rate_response_dict = tax_rate_response_instance.to_dict()
# create an instance of TaxRateResponse from a dict
tax_rate_response_from_dict = TaxRateResponse.from_dict(tax_rate_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


