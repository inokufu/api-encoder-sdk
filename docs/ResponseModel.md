# ResponseModel


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index** | **str** | Index of the query : must be unique | 
**query** | **str** | User query | 
**vector** | **List[float]** | Vector representation of the query | [optional] [default to []]

## Example

```python
from inokufu_encoder_client.models.response_model import ResponseModel

# TODO update the JSON string below
json = "{}"
# create an instance of ResponseModel from a JSON string
response_model_instance = ResponseModel.from_json(json)
# print the JSON string representation of the object
print ResponseModel.to_json()

# convert the object into a dict
response_model_dict = response_model_instance.to_dict()
# create an instance of ResponseModel from a dict
response_model_form_dict = response_model.from_dict(response_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


