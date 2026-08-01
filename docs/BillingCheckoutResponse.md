# BillingCheckoutResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BillingCheckoutData**](BillingCheckoutData.md) |  | 

## Example

```python
from invoicepdfs.models.billing_checkout_response import BillingCheckoutResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BillingCheckoutResponse from a JSON string
billing_checkout_response_instance = BillingCheckoutResponse.from_json(json)
# print the JSON string representation of the object
print(BillingCheckoutResponse.to_json())

# convert the object into a dict
billing_checkout_response_dict = billing_checkout_response_instance.to_dict()
# create an instance of BillingCheckoutResponse from a dict
billing_checkout_response_from_dict = BillingCheckoutResponse.from_dict(billing_checkout_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


