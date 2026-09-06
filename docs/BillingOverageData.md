# BillingOverageData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**overage_enabled** | **bool** |  | 
**overage_available** | **bool** |  | 
**overage_price_millicents** | **int** |  | [optional] 

## Example

```python
from invoicepdfs.models.billing_overage_data import BillingOverageData

# TODO update the JSON string below
json = "{}"
# create an instance of BillingOverageData from a JSON string
billing_overage_data_instance = BillingOverageData.from_json(json)
# print the JSON string representation of the object
print(BillingOverageData.to_json())

# convert the object into a dict
billing_overage_data_dict = billing_overage_data_instance.to_dict()
# create an instance of BillingOverageData from a dict
billing_overage_data_from_dict = BillingOverageData.from_dict(billing_overage_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


