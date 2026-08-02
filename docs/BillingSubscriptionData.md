# BillingSubscriptionData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**plan_id** | **str** |  | 
**plan_name** | **str** |  | 
**stripe_configured** | **bool** |  | [optional] [default to False]
**has_billing_account** | **bool** |  | [optional] [default to False]

## Example

```python
from invoicepdfs.models.billing_subscription_data import BillingSubscriptionData

# TODO update the JSON string below
json = "{}"
# create an instance of BillingSubscriptionData from a JSON string
billing_subscription_data_instance = BillingSubscriptionData.from_json(json)
# print the JSON string representation of the object
print(BillingSubscriptionData.to_json())

# convert the object into a dict
billing_subscription_data_dict = billing_subscription_data_instance.to_dict()
# create an instance of BillingSubscriptionData from a dict
billing_subscription_data_from_dict = BillingSubscriptionData.from_dict(billing_subscription_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


