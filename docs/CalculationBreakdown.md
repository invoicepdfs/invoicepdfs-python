# CalculationBreakdown


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subtotal** | [**Money**](Money.md) |  | 
**discount_total** | [**Money**](Money.md) |  | 
**tax_total** | [**Money**](Money.md) |  | 
**shipping_total** | [**Money**](Money.md) |  | 
**total** | [**Money**](Money.md) |  | 

## Example

```python
from invoicepdfs.models.calculation_breakdown import CalculationBreakdown

# TODO update the JSON string below
json = "{}"
# create an instance of CalculationBreakdown from a JSON string
calculation_breakdown_instance = CalculationBreakdown.from_json(json)
# print the JSON string representation of the object
print(CalculationBreakdown.to_json())

# convert the object into a dict
calculation_breakdown_dict = calculation_breakdown_instance.to_dict()
# create an instance of CalculationBreakdown from a dict
calculation_breakdown_from_dict = CalculationBreakdown.from_dict(calculation_breakdown_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


