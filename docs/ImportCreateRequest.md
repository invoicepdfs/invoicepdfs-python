# ImportCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source_format** | **str** |  | 
**data** | **List[Dict[str, object]]** |  | 

## Example

```python
from invoicepdfs.models.import_create_request import ImportCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ImportCreateRequest from a JSON string
import_create_request_instance = ImportCreateRequest.from_json(json)
# print the JSON string representation of the object
print(ImportCreateRequest.to_json())

# convert the object into a dict
import_create_request_dict = import_create_request_instance.to_dict()
# create an instance of ImportCreateRequest from a dict
import_create_request_from_dict = ImportCreateRequest.from_dict(import_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


