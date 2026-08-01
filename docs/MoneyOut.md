# MoneyOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**currency** | **str** |  | 

## Example

```python
from invoicepdfs.models.money_out import MoneyOut

# TODO update the JSON string below
json = "{}"
# create an instance of MoneyOut from a JSON string
money_out_instance = MoneyOut.from_json(json)
# print the JSON string representation of the object
print(MoneyOut.to_json())

# convert the object into a dict
money_out_dict = money_out_instance.to_dict()
# create an instance of MoneyOut from a dict
money_out_from_dict = MoneyOut.from_dict(money_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


