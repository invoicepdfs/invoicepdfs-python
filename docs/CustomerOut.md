# CustomerOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**tax_id** | **str** |  | [optional] 
**billing_address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**shipping_address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**metadata** | **Dict[str, object]** |  | [optional] 
**id** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.customer_out import CustomerOut

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerOut from a JSON string
customer_out_instance = CustomerOut.from_json(json)
# print the JSON string representation of the object
print(CustomerOut.to_json())

# convert the object into a dict
customer_out_dict = customer_out_instance.to_dict()
# create an instance of CustomerOut from a dict
customer_out_from_dict = CustomerOut.from_dict(customer_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


