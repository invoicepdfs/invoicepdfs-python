# ApiKeyListItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**last4** | **str** |  | 
**created_at** | **str** |  | 
**revoked_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.api_key_list_item import ApiKeyListItem

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyListItem from a JSON string
api_key_list_item_instance = ApiKeyListItem.from_json(json)
# print the JSON string representation of the object
print(ApiKeyListItem.to_json())

# convert the object into a dict
api_key_list_item_dict = api_key_list_item_instance.to_dict()
# create an instance of ApiKeyListItem from a dict
api_key_list_item_from_dict = ApiKeyListItem.from_dict(api_key_list_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


