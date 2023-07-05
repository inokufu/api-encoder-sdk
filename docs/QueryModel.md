# QueryModel


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index** | **str** | Index of the query : must be unique | 
**query** | **str** | User query | 
**lang** | [**LangEnum**](LangEnum.md) |  | 

## Example

```python
from inokufu_encoder_client.models.query_model import QueryModel

# TODO update the JSON string below
json = "{}"
# create an instance of QueryModel from a JSON string
query_model_instance = QueryModel.from_json(json)
# print the JSON string representation of the object
print QueryModel.to_json()

# convert the object into a dict
query_model_dict = query_model_instance.to_dict()
# create an instance of QueryModel from a dict
query_model_form_dict = query_model.from_dict(query_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


