# BillingCheckoutRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**price_id** | **str** | Stripe price ID for the plan | 

## Example

```python
from invoicepdfs.models.billing_checkout_request import BillingCheckoutRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BillingCheckoutRequest from a JSON string
billing_checkout_request_instance = BillingCheckoutRequest.from_json(json)
# print the JSON string representation of the object
print(BillingCheckoutRequest.to_json())

# convert the object into a dict
billing_checkout_request_dict = billing_checkout_request_instance.to_dict()
# create an instance of BillingCheckoutRequest from a dict
billing_checkout_request_from_dict = BillingCheckoutRequest.from_dict(billing_checkout_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


