# BillingSubscriptionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BillingSubscriptionData**](BillingSubscriptionData.md) |  | 

## Example

```python
from invoicepdfs.models.billing_subscription_response import BillingSubscriptionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BillingSubscriptionResponse from a JSON string
billing_subscription_response_instance = BillingSubscriptionResponse.from_json(json)
# print the JSON string representation of the object
print(BillingSubscriptionResponse.to_json())

# convert the object into a dict
billing_subscription_response_dict = billing_subscription_response_instance.to_dict()
# create an instance of BillingSubscriptionResponse from a dict
billing_subscription_response_from_dict = BillingSubscriptionResponse.from_dict(billing_subscription_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


