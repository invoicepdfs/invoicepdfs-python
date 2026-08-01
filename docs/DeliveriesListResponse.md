# DeliveriesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DeliveryOut]**](DeliveryOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.deliveries_list_response import DeliveriesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveriesListResponse from a JSON string
deliveries_list_response_instance = DeliveriesListResponse.from_json(json)
# print the JSON string representation of the object
print(DeliveriesListResponse.to_json())

# convert the object into a dict
deliveries_list_response_dict = deliveries_list_response_instance.to_dict()
# create an instance of DeliveriesListResponse from a dict
deliveries_list_response_from_dict = DeliveriesListResponse.from_dict(deliveries_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


