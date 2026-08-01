# ImportOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**source_format** | **str** |  | 
**status** | **str** |  | 
**total_rows** | **int** |  | 
**imported_rows** | **int** |  | 
**failed_rows** | **int** |  | 
**errors** | **List[Dict[str, object]]** |  | [optional] 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**completed_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.import_out import ImportOut

# TODO update the JSON string below
json = "{}"
# create an instance of ImportOut from a JSON string
import_out_instance = ImportOut.from_json(json)
# print the JSON string representation of the object
print(ImportOut.to_json())

# convert the object into a dict
import_out_dict = import_out_instance.to_dict()
# create an instance of ImportOut from a dict
import_out_from_dict = ImportOut.from_dict(import_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


