# CountryOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from invoicepdfs.models.country_out import CountryOut

# TODO update the JSON string below
json = "{}"
# create an instance of CountryOut from a JSON string
country_out_instance = CountryOut.from_json(json)
# print the JSON string representation of the object
print(CountryOut.to_json())

# convert the object into a dict
country_out_dict = country_out_instance.to_dict()
# create an instance of CountryOut from a dict
country_out_from_dict = CountryOut.from_dict(country_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


