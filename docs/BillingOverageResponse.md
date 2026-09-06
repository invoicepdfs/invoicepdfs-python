# BillingOverageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BillingOverageData**](BillingOverageData.md) |  | 

## Example

```python
from invoicepdfs.models.billing_overage_response import BillingOverageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BillingOverageResponse from a JSON string
billing_overage_response_instance = BillingOverageResponse.from_json(json)
# print the JSON string representation of the object
print(BillingOverageResponse.to_json())

# convert the object into a dict
billing_overage_response_dict = billing_overage_response_instance.to_dict()
# create an instance of BillingOverageResponse from a dict
billing_overage_response_from_dict = BillingOverageResponse.from_dict(billing_overage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


