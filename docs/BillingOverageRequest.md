# BillingOverageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Whether renders past the monthly quota should be billed | 

## Example

```python
from invoicepdfs.models.billing_overage_request import BillingOverageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BillingOverageRequest from a JSON string
billing_overage_request_instance = BillingOverageRequest.from_json(json)
# print the JSON string representation of the object
print(BillingOverageRequest.to_json())

# convert the object into a dict
billing_overage_request_dict = billing_overage_request_instance.to_dict()
# create an instance of BillingOverageRequest from a dict
billing_overage_request_from_dict = BillingOverageRequest.from_dict(billing_overage_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


