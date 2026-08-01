# BillingCheckoutData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **str** |  | 
**url** | **str** |  | 

## Example

```python
from invoicepdfs.models.billing_checkout_data import BillingCheckoutData

# TODO update the JSON string below
json = "{}"
# create an instance of BillingCheckoutData from a JSON string
billing_checkout_data_instance = BillingCheckoutData.from_json(json)
# print the JSON string representation of the object
print(BillingCheckoutData.to_json())

# convert the object into a dict
billing_checkout_data_dict = billing_checkout_data_instance.to_dict()
# create an instance of BillingCheckoutData from a dict
billing_checkout_data_from_dict = BillingCheckoutData.from_dict(billing_checkout_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


