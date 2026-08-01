# JobOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**type** | **str** |  | 
**status** | **str** |  | 
**progress** | [**JobProgressOut**](JobProgressOut.md) |  | 
**result** | **Dict[str, object]** |  | [optional] 
**error** | **str** |  | [optional] 
**created_at** | **str** |  | 
**started_at** | **str** |  | [optional] 
**completed_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.job_out import JobOut

# TODO update the JSON string below
json = "{}"
# create an instance of JobOut from a JSON string
job_out_instance = JobOut.from_json(json)
# print the JSON string representation of the object
print(JobOut.to_json())

# convert the object into a dict
job_out_dict = job_out_instance.to_dict()
# create an instance of JobOut from a dict
job_out_from_dict = JobOut.from_dict(job_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


