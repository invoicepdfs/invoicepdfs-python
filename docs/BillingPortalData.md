# BillingPortalData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | 

## Example

```python
from invoicepdfs.models.billing_portal_data import BillingPortalData

# TODO update the JSON string below
json = "{}"
# create an instance of BillingPortalData from a JSON string
billing_portal_data_instance = BillingPortalData.from_json(json)
# print the JSON string representation of the object
print(BillingPortalData.to_json())

# convert the object into a dict
billing_portal_data_dict = billing_portal_data_instance.to_dict()
# create an instance of BillingPortalData from a dict
billing_portal_data_from_dict = BillingPortalData.from_dict(billing_portal_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


