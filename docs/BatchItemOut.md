# BatchItemOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**external_id** | **str** |  | [optional] 
**document_type** | **str** |  | 
**status** | **str** |  | 
**render_id** | **str** |  | [optional] 
**error_message** | **str** |  | [optional] 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.batch_item_out import BatchItemOut

# TODO update the JSON string below
json = "{}"
# create an instance of BatchItemOut from a JSON string
batch_item_out_instance = BatchItemOut.from_json(json)
# print the JSON string representation of the object
print(BatchItemOut.to_json())

# convert the object into a dict
batch_item_out_dict = batch_item_out_instance.to_dict()
# create an instance of BatchItemOut from a dict
batch_item_out_from_dict = BatchItemOut.from_dict(batch_item_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


