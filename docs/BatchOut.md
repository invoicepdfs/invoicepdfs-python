# BatchOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**operation** | **str** |  | 
**template_id** | **str** |  | 
**total_items** | **int** |  | 
**completed_items** | **int** |  | 
**failed_items** | **int** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**completed_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.batch_out import BatchOut

# TODO update the JSON string below
json = "{}"
# create an instance of BatchOut from a JSON string
batch_out_instance = BatchOut.from_json(json)
# print the JSON string representation of the object
print(BatchOut.to_json())

# convert the object into a dict
batch_out_dict = batch_out_instance.to_dict()
# create an instance of BatchOut from a dict
batch_out_from_dict = BatchOut.from_dict(batch_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


