# JobProgressOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current** | **int** |  | 
**total** | **int** |  | 
**percentage** | **int** |  | 

## Example

```python
from invoicepdfs.models.job_progress_out import JobProgressOut

# TODO update the JSON string below
json = "{}"
# create an instance of JobProgressOut from a JSON string
job_progress_out_instance = JobProgressOut.from_json(json)
# print the JSON string representation of the object
print(JobProgressOut.to_json())

# convert the object into a dict
job_progress_out_dict = job_progress_out_instance.to_dict()
# create an instance of JobProgressOut from a dict
job_progress_out_from_dict = JobProgressOut.from_dict(job_progress_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


