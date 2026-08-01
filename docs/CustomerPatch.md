# CustomerPatch


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**tax_id** | **str** |  | [optional] 
**billing_address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**shipping_address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**metadata** | **Dict[str, object]** |  | [optional] 

## Example

```python
from invoicepdfs.models.customer_patch import CustomerPatch

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerPatch from a JSON string
customer_patch_instance = CustomerPatch.from_json(json)
# print the JSON string representation of the object
print(CustomerPatch.to_json())

# convert the object into a dict
customer_patch_dict = customer_patch_instance.to_dict()
# create an instance of CustomerPatch from a dict
customer_patch_from_dict = CustomerPatch.from_dict(customer_patch_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


