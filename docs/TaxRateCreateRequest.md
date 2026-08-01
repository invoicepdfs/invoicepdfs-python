# TaxRateCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**rate** | **str** |  | 
**inclusive** | **bool** |  | [optional] [default to False]
**jurisdiction** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.tax_rate_create_request import TaxRateCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRateCreateRequest from a JSON string
tax_rate_create_request_instance = TaxRateCreateRequest.from_json(json)
# print the JSON string representation of the object
print(TaxRateCreateRequest.to_json())

# convert the object into a dict
tax_rate_create_request_dict = tax_rate_create_request_instance.to_dict()
# create an instance of TaxRateCreateRequest from a dict
tax_rate_create_request_from_dict = TaxRateCreateRequest.from_dict(tax_rate_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


