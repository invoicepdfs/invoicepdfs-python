# BillingPlan


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**price_id** | **str** |  | 
**monthly_render_quota** | **int** |  | 

## Example

```python
from invoicepdfs.models.billing_plan import BillingPlan

# TODO update the JSON string below
json = "{}"
# create an instance of BillingPlan from a JSON string
billing_plan_instance = BillingPlan.from_json(json)
# print the JSON string representation of the object
print(BillingPlan.to_json())

# convert the object into a dict
billing_plan_dict = billing_plan_instance.to_dict()
# create an instance of BillingPlan from a dict
billing_plan_from_dict = BillingPlan.from_dict(billing_plan_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


