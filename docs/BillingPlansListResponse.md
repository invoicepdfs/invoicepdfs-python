# BillingPlansListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BillingPlan]**](BillingPlan.md) |  | 

## Example

```python
from invoicepdfs.models.billing_plans_list_response import BillingPlansListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BillingPlansListResponse from a JSON string
billing_plans_list_response_instance = BillingPlansListResponse.from_json(json)
# print the JSON string representation of the object
print(BillingPlansListResponse.to_json())

# convert the object into a dict
billing_plans_list_response_dict = billing_plans_list_response_instance.to_dict()
# create an instance of BillingPlansListResponse from a dict
billing_plans_list_response_from_dict = BillingPlansListResponse.from_dict(billing_plans_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


