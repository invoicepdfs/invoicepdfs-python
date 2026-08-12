# CountriesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CountryOut]**](CountryOut.md) |  | 

## Example

```python
from invoicepdfs.models.countries_list_response import CountriesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CountriesListResponse from a JSON string
countries_list_response_instance = CountriesListResponse.from_json(json)
# print the JSON string representation of the object
print(CountriesListResponse.to_json())

# convert the object into a dict
countries_list_response_dict = countries_list_response_instance.to_dict()
# create an instance of CountriesListResponse from a dict
countries_list_response_from_dict = CountriesListResponse.from_dict(countries_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


