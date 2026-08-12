# PageSizeOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**width_mm** | **float** |  | 
**height_mm** | **float** |  | 

## Example

```python
from invoicepdfs.models.page_size_out import PageSizeOut

# TODO update the JSON string below
json = "{}"
# create an instance of PageSizeOut from a JSON string
page_size_out_instance = PageSizeOut.from_json(json)
# print the JSON string representation of the object
print(PageSizeOut.to_json())

# convert the object into a dict
page_size_out_dict = page_size_out_instance.to_dict()
# create an instance of PageSizeOut from a dict
page_size_out_from_dict = PageSizeOut.from_dict(page_size_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


