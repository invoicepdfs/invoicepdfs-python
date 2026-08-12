# CurrencyOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**name** | **str** |  | 
**symbol** | **str** |  | 
**decimals** | **int** |  | 

## Example

```python
from invoicepdfs.models.currency_out import CurrencyOut

# TODO update the JSON string below
json = "{}"
# create an instance of CurrencyOut from a JSON string
currency_out_instance = CurrencyOut.from_json(json)
# print the JSON string representation of the object
print(CurrencyOut.to_json())

# convert the object into a dict
currency_out_dict = currency_out_instance.to_dict()
# create an instance of CurrencyOut from a dict
currency_out_from_dict = CurrencyOut.from_dict(currency_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


